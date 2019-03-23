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
ms.openlocfilehash: 700e6d24e49cf11bf91780895f5a796cc1d8349d
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753435"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="563a5-102">Løse problemer med å dele SharePoint-innhold med eksterne brukere</span><span class="sxs-lookup"><span data-stu-id="563a5-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="563a5-103">Kontroller at eksterne deling er aktivert for organisasjonen:</span><span class="sxs-lookup"><span data-stu-id="563a5-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="563a5-104">Gå til den [tjenester &amp; tillegg side i administrasjonssenteret for Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), og klikk **områder**.</span><span class="sxs-lookup"><span data-stu-id="563a5-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="563a5-105">Kontroller at innstillingen slås til "On".</span><span class="sxs-lookup"><span data-stu-id="563a5-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="563a5-106">Hvis "Bare eksisterende eksterne brukere" er valgt, må du kontrollere at den eksterne brukeren er oppført i administrasjonssenteret for Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="563a5-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="563a5-107">Kontroller at eksternt delingen som er aktivert for området.</span><span class="sxs-lookup"><span data-stu-id="563a5-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="563a5-108">For en klassisk områdesamling:</span><span class="sxs-lookup"><span data-stu-id="563a5-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="563a5-109">Klikk **områdesamlinger**i klassisk SharePoint administrasjonssenteret, i ruten til venstre.</span><span class="sxs-lookup"><span data-stu-id="563a5-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="563a5-110">Velg område eller områder, og klikk **Deling**på båndet.</span><span class="sxs-lookup"><span data-stu-id="563a5-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="563a5-111">For et gruppeområde som tilhører en gruppe for Office 365, eller et område for kommunikasjon:</span><span class="sxs-lookup"><span data-stu-id="563a5-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="563a5-112">Slike området har den samme delte innstillingen som innstilling for bedriften, med mindre innstillingen for hele organisasjonen kan dele filer ved hjelp av koblinger som ikke krever pålogging.</span><span class="sxs-lookup"><span data-stu-id="563a5-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="563a5-113">I dette tilfellet Tillat områdene deling med nye og eksisterende eksterne brukere som logger på.</span><span class="sxs-lookup"><span data-stu-id="563a5-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="563a5-114">Hvis du vil endre innstillingen for bestemte områder, bruke den nye SharePoint-administrasjonssenteret (forhåndsvisning) eller PowerShell.</span><span class="sxs-lookup"><span data-stu-id="563a5-114">To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell.</span></span> <span data-ttu-id="563a5-115">[Lær mer](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="563a5-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="563a5-116">Eksterne delte innstillingen for et område kan være mer restriktive enn innstillingene for hele organisasjonen, men ikke mer tillatte DACLer enn innstillingen for hele organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="563a5-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

