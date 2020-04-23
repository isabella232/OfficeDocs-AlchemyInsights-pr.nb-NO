---
title: Et av dine lokale Federation Service Sertifikater utløper
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: dafa344ec649002900e98a5e183b3e5f759707e1
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785312"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="5cb2a-102">Et av dine lokale Federation Service Sertifikater utløper</span><span class="sxs-lookup"><span data-stu-id="5cb2a-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="5cb2a-103">Hvis du vil løse dette problemet, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="5cb2a-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="5cb2a-104">Installer Microsoft Azure Active Directory-modul for Windows PowerShell på datamaskinen (hvis modulen ikke allerede er installert).</span><span class="sxs-lookup"><span data-stu-id="5cb2a-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="5cb2a-105">Hvis du vil gjøre dette, kan du gå til [Azure Active Directory PowerShell for Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="5cb2a-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="5cb2a-106">Følg trinnene i delen "Scenario 1: AD FS tokensigneringssertifikatet er utløpt" i ["Det oppstod et problem under tilgang til området" fra AD FS når en samlet bruker logger på Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="5cb2a-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="5cb2a-107">Følg trinnene i [Slik oppdaterer eller reparerer du innstillingene for et forent domene i Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="5cb2a-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="5cb2a-108">Hvis du vil ha mer informasjon om fornyelse av Federation-sertifikater, kan du se [Sertifikatfornyelse for O365 og Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="5cb2a-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

