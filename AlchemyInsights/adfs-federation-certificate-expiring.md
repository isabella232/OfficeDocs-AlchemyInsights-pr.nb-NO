---
title: ADFS Federation sertifikat utløper
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737198"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="9db8a-102">ADFS Federation sertifikat utløper</span><span class="sxs-lookup"><span data-stu-id="9db8a-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="9db8a-103">Hvis du vil løse dette problemet, følger du denne fremgangsmåten:</span><span class="sxs-lookup"><span data-stu-id="9db8a-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="9db8a-104">Installere Microsoft Azure Active Directory-modul for Windows PowerShell på datamaskinen (Hvis modulen ikke allerede er installert).</span><span class="sxs-lookup"><span data-stu-id="9db8a-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="9db8a-105">Hvis du vil gjøre dette, kan du gå til [Administrer Azure ad ved hjelp av Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="9db8a-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="9db8a-106">Følg trinnene i den "scenario 1: AD FS token signeringssertifikatet er utløpt" delen av ["det oppstod et problem under tilgang til området" feil fra AD FS når en forent bruker logger på Office 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="9db8a-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="9db8a-107">Følg trinnene i [oppdatere eller reparere innstillingene for et forent domene i Office 365, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="9db8a-107">Follow the steps in [Update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="9db8a-108">Hvis du vil ha mer informasjon om fornyelse av Federation sertifikater, kan du se [fornye Federation sertifikater for Office 365 og Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="9db8a-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
