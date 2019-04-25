---
title: Deling med eksterne brukere fungerer ikke
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32369507"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="04c20-102">Løse problemer med å dele SharePoint-innhold med eksterne brukere</span><span class="sxs-lookup"><span data-stu-id="04c20-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="04c20-103">Kontroller at eksterne deling er aktivert for organisasjonen:</span><span class="sxs-lookup"><span data-stu-id="04c20-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="04c20-104">Gå til den [tjenester &amp; tillegg side i administrasjonssenteret for Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), og klikk **områder**.</span><span class="sxs-lookup"><span data-stu-id="04c20-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="04c20-105">Kontroller at innstillingen slås til "On".</span><span class="sxs-lookup"><span data-stu-id="04c20-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="04c20-106">Hvis "Bare eksisterende eksterne brukere" er valgt, må du kontrollere at den eksterne brukeren er oppført i administrasjonssenteret for Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="04c20-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="04c20-107">Kontroller at eksternt delingen som er aktivert for området.</span><span class="sxs-lookup"><span data-stu-id="04c20-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="04c20-108">For en klassisk områdesamling:</span><span class="sxs-lookup"><span data-stu-id="04c20-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="04c20-109">Klikk **områder**i nye SharePoint administrasjonssenteret, i ruten til venstre.</span><span class="sxs-lookup"><span data-stu-id="04c20-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="04c20-110">Velg område eller områder, og klikk **Deling**på båndet.</span><span class="sxs-lookup"><span data-stu-id="04c20-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="04c20-111">For et gruppeområde som tilhører en gruppe for Office 365, eller et område for kommunikasjon:</span><span class="sxs-lookup"><span data-stu-id="04c20-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="04c20-112">Slike området har den samme delte innstillingen som innstilling for bedriften, med mindre innstillingen for hele organisasjonen kan dele filer ved hjelp av koblinger som ikke krever pålogging.</span><span class="sxs-lookup"><span data-stu-id="04c20-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="04c20-113">I dette tilfellet Tillat områdene deling med nye og eksisterende eksterne brukere som logger på.</span><span class="sxs-lookup"><span data-stu-id="04c20-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="04c20-114">Hvis du vil endre innstillingen for bestemte områder, kan du bruke den nye SharePoint-administrasjonssenteret eller PowerShell.</span><span class="sxs-lookup"><span data-stu-id="04c20-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="04c20-115">[Lær mer](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="04c20-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="04c20-116">Eksterne delte innstillingen for et område kan være mer restriktive enn innstillingene for hele organisasjonen, men ikke mer tillatte DACLer enn innstillingen for hele organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="04c20-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

