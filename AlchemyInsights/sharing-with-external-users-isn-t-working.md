---
title: Deling med eksterne brukere fungerer ikke
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 37da77c73b3abbdcf9cb2b9c4c43f31eea3c0a49
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/27/2020
ms.locfileid: "43913011"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="70386-102">Løse problemer med å dele SharePoint-innhold med eksterne brukere</span><span class="sxs-lookup"><span data-stu-id="70386-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="70386-103">Kontroller at ekstern deling er aktivert for organisasjonen:</span><span class="sxs-lookup"><span data-stu-id="70386-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="70386-104">Gå til [ &amp; siden Tjenester-tillegg i administrasjonssenteret for Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), og klikk **Områder**.</span><span class="sxs-lookup"><span data-stu-id="70386-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="70386-105">Kontroller at innstillingen er slått til "På".</span><span class="sxs-lookup"><span data-stu-id="70386-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="70386-106">Hvis "Bare eksisterende eksterne brukere" er valgt, må du kontrollere at den eksterne brukeren er oppført i administrasjonssenteret for Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="70386-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="70386-107">Kontroller at ekstern deling den er slått på for området.</span><span class="sxs-lookup"><span data-stu-id="70386-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="70386-108">For en klassisk områdesamling:</span><span class="sxs-lookup"><span data-stu-id="70386-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="70386-109">Klikk **områder**i ruten til venstre i det nye administrasjonssenteret for SharePoint.</span><span class="sxs-lookup"><span data-stu-id="70386-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="70386-110">Velg området eller områdene, og klikk **Deling**på båndet.</span><span class="sxs-lookup"><span data-stu-id="70386-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="70386-111">For et gruppeområde som tilhører en Microsoft 365-gruppe eller et kommunikasjonsområde:</span><span class="sxs-lookup"><span data-stu-id="70386-111">For a team site that belongs to an Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="70386-112">Disse nye områdetypene har samme delingsinnstilling som innstillingen for hele organisasjonen, med mindre innstillingen for hele organisasjonen gjør det mulig å dele filer ved hjelp av koblinger som ikke krever pålogging.</span><span class="sxs-lookup"><span data-stu-id="70386-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="70386-113">I dette tilfellet tillater nettstedene deling med nye og eksisterende eksterne brukere som logger på.</span><span class="sxs-lookup"><span data-stu-id="70386-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="70386-114">Hvis du vil endre innstillingen for bestemte områder, bruker du det nye administrasjonssenteret for SharePoint eller PowerShell.</span><span class="sxs-lookup"><span data-stu-id="70386-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="70386-115">[Finn ut mer](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="70386-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="70386-116">Innstillingen for ekstern deling for alle nettsteder kan være mer restriktive enn innstillingen for hele organisasjonen, men ikke mer tillatt enn innstillingen for hele organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="70386-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

