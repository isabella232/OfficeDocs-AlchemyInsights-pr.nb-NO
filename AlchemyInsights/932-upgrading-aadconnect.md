---
title: 932 oppgraderer AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9add88a0e4a2590639cbfc546afdcdf5e6aa4886
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29481974"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="a5552-102">Oppgradering Azure AD koble</span><span class="sxs-lookup"><span data-stu-id="a5552-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="a5552-p101">Som standard aktiveres automatisk oppgradering for Azure AD-tilkobling, som bidrar til å sikre at du kjører den nyeste versjonen. Hvis du vil kontrollere innstillingene for automatisk oppgradering, kan du bruke cmdleten **Get-ADSyncAutoUpgrade** i Azure AD PowerShell. Cmdleten vil returnere en av følgende verdier:</span><span class="sxs-lookup"><span data-stu-id="a5552-p101">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version. To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell. The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="a5552-106">**Aktivert**: automatisk oppgradering er aktivert.</span><span class="sxs-lookup"><span data-stu-id="a5552-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="a5552-107">**Deaktivert**: automatisk oppgradering er deaktivert.</span><span class="sxs-lookup"><span data-stu-id="a5552-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="a5552-p102">**Suspended**: systemet er ikke lenger berettiget til å motta automatiske oppgraderinger. Du kan ikke konfigurere denne verdien. Det er satt av systemet.</span><span class="sxs-lookup"><span data-stu-id="a5552-p102">**Suspended**: The system is no longer eligible to receive automatic upgrades. You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="a5552-110">Hvis du vil ha mer informasjon, kan du se [automatisk oppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="a5552-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="a5552-111">Hvis du vil laste ned den nyeste versjonen av Azure AD-tilkobling, kan du gå til [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="a5552-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

