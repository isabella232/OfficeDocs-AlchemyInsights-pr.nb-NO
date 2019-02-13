---
title: Ett av sertifikatene dine lokale Federation Service er utløpt
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: bed33ba4d09fe4598c5e73eb21f0af1b7670f4c1
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29914409"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="36d23-102">Ett av sertifikatene dine lokale Federation Service er utløpt</span><span class="sxs-lookup"><span data-stu-id="36d23-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="36d23-103">Hvis du vil løse dette problemet, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="36d23-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="36d23-p101">Installere det Microsoft Azure Active Directory-modulen for Windows PowerShell på datamaskinen (Hvis modulen ikke er allerede installert). Hvis du vil gjøre dette, kan du gå til [Azure Active Directory PowerShell for diagram](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="36d23-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="36d23-106">Følg trinnene i den "Scenario 1: AD FS token signere sertifikatet er utløpt" delen av ["Det oppstod en feil under tilgang til området" feil fra AD FS når en forent bruker logger på Office 365, Azure, eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="36d23-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="36d23-107">Følg trinnene i t[hvordan å oppdatere eller reparere innstillingene for medlemmer av organisasjonsnettverk domene i Office 365, Azure, eller Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="36d23-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="36d23-108">Hvis du vil ha mer informasjon om å fornye Federation sertifikater, kan du se [sertifikatfornyelse for O365 og Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="36d23-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

