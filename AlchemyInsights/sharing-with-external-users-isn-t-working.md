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
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502240"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="a0717-102">Løs problemer med deling av SharePoint-innhold med eksterne brukere</span><span class="sxs-lookup"><span data-stu-id="a0717-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="a0717-103">Kontroller at ekstern deling er slått på for organisasjonen:</span><span class="sxs-lookup"><span data-stu-id="a0717-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="a0717-104">Gå til [siden tjenester &amp; -tillegg i administrasjonssenteret for Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), og klikk **områder**.</span><span class="sxs-lookup"><span data-stu-id="a0717-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="a0717-105">Kontroller at innstillingen er slått på "på".</span><span class="sxs-lookup"><span data-stu-id="a0717-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="a0717-106">Hvis "bare eksisterende eksterne brukere" er valgt, må du kontrollere at den eksterne brukeren er oppført i administrasjonssenteret for Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a0717-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="a0717-107">Kontroller at ekstern deling den er slått på for området.</span><span class="sxs-lookup"><span data-stu-id="a0717-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="a0717-108">For en klassisk områdesamling:</span><span class="sxs-lookup"><span data-stu-id="a0717-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="a0717-109">Klikk **områder**i ruten til venstre i det nye administrasjonssenteret for SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a0717-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="a0717-110">Velg området eller områdene, og klikk **deling**på båndet.</span><span class="sxs-lookup"><span data-stu-id="a0717-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="a0717-111">For et gruppeområde som tilhører en Office 365-gruppe, eller et område for kommunikasjon:</span><span class="sxs-lookup"><span data-stu-id="a0717-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="a0717-112">Disse nye områdetypene har samme Delings innstilling som innstillingen for hele organisasjonen, med mindre innstillingen for hele organisasjonen tillater deling av filer ved hjelp av koblinger som ikke krever pålogging.</span><span class="sxs-lookup"><span data-stu-id="a0717-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="a0717-113">I dette tilfellet tillater områdene deling med nye og eksisterende eksterne brukere som logger på.</span><span class="sxs-lookup"><span data-stu-id="a0717-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="a0717-114">Hvis du vil endre innstillingen for bestemte områder, kan du bruke det nye administrasjonssenteret for SharePoint eller PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a0717-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="a0717-115">[Finn ut mer](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="a0717-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="a0717-116">Innstillingen for ekstern deling for et hvilket som helst område kan være mer begrenset enn innstillingen for hele organisasjonen, men ikke mer ettergivende enn innstillingen for hele organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="a0717-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

