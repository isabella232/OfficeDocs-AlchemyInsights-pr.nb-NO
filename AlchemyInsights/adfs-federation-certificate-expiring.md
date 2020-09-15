---
title: Sertifikat utløp for ADFS-forbund
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686754"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="a2374-102">Sertifikat utløp for ADFS-forbund</span><span class="sxs-lookup"><span data-stu-id="a2374-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="a2374-103">Følg denne Fremgangs måten for å løse dette problemet:</span><span class="sxs-lookup"><span data-stu-id="a2374-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="a2374-104">Installer Microsoft Azure Active Directory-modulen for Windows PowerShell på data maskinen (Hvis modulen ikke allerede er installert).</span><span class="sxs-lookup"><span data-stu-id="a2374-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="a2374-105">Hvis du vil gjøre dette, går du til [administrere Azure ad ved hjelp av Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="a2374-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="a2374-106">Følg Fremgangs måten i delen "scenario 1: signerings sertifikatet for AD FS token utløpt" i [«det oppstod et problem under tilgang til nettstedet» fra AD FS når en Forbunds bruker logger seg på Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="a2374-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="a2374-107">Følg trinnene i [oppdatere eller reparere innstillingene for et organisasjons domene i Microsoft, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="a2374-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="a2374-108">Hvis du vil vite mer om hvordan du fornyer forbundede sertifikater, kan du se [fornye forbundede sertifikater for Microsoft 365 og Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)</span><span class="sxs-lookup"><span data-stu-id="a2374-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
