---
title: ADFS-forbundssertifikat utløper
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821960"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="73465-102">ADFS-forbundssertifikat utløper</span><span class="sxs-lookup"><span data-stu-id="73465-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="73465-103">Følg disse trinnene for å løse dette problemet:</span><span class="sxs-lookup"><span data-stu-id="73465-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="73465-104">Installer Microsoft Azure Active Directory-modulen for Windows PowerShell på datamaskinen (hvis modulen ikke allerede er installert).</span><span class="sxs-lookup"><span data-stu-id="73465-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="73465-105">Dette gjør du ved å gå til [Administrere Azure AD ved hjelp av Windows PowerShell.](https://aka.ms/aadposh)</span><span class="sxs-lookup"><span data-stu-id="73465-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="73465-106">Følg fremgangsmåten i avsnittet «Scenario 1: AD FS token-signeringssertifikatet er utløpt» i feilmeldingen «Det oppstod et problem med tilgang til nettstedet» fra AD FS når en bruker i forbund logger på [Microsoft 365, Azure eller Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="73465-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="73465-107">Følg fremgangsmåten i Oppdatere eller reparere innstillingene for et domene i forbund [i Microsoft, Azure eller Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)</span><span class="sxs-lookup"><span data-stu-id="73465-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="73465-108">Hvis du vil lære mer om fornyelse av forbundssertifikater, kan du se Fornye [forbundssertifikater for Microsoft 365 og Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="73465-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
