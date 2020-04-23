---
title: Feilsøke ingen meldinger om tilgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759809"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="eff88-102">Feilsøke ingen meldinger om tilgang</span><span class="sxs-lookup"><span data-stu-id="eff88-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="eff88-103">Hvis noen fikk meldingen "Ingen tilgang" til en delt mappe i SharePoint, kan administratoren for områdesamlingen ha aktivert "Begrenset tilgang til brukertillatelselockdown-modus."</span><span class="sxs-lookup"><span data-stu-id="eff88-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="eff88-104">Slik slår du av dette:</span><span class="sxs-lookup"><span data-stu-id="eff88-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="eff88-105">Bla til området, klikk Innstillinger-ikonet, og klikk deretter **Innstillinger for område**.</span><span class="sxs-lookup"><span data-stu-id="eff88-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="eff88-106">Klikk Funksjoner for **områdesamling under** **Administrasjon av områdesamling**.</span><span class="sxs-lookup"><span data-stu-id="eff88-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="eff88-107">**Klikk**Deaktiver ved siden av **begrenset tilgang til låsemodus for brukertillatelser**for begrenset tilgang .</span><span class="sxs-lookup"><span data-stu-id="eff88-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="eff88-108">En melding om ingen tilgang kan også forekomme for delte mapper hvis området er et publiseringsområde.</span><span class="sxs-lookup"><span data-stu-id="eff88-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="eff88-109">Hvis du vil ha mer informasjon, kan du se [Ingen tilgang til Access når du åpner en delt mappe](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="eff88-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="eff88-110">Hvis noen fikk meldingen "Ingen tilgang" når du prøver å vise tilgangsforespørsler, må brukeren legges til som administrator for en områdesamling eller et medlem av Eiere-gruppen for området.</span><span class="sxs-lookup"><span data-stu-id="eff88-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="eff88-111">Hvis du vil ha mer informasjon, kan du se [Ingen tilgang til listen over tilgangsforespørsler](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="eff88-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="eff88-112">Hvis en bruker fikk feilmeldingen "Ingen tilgang" etter at de ble fjernet fra Active Directory lokalt og deretter lagt til igjen, kan du se [Ingen tilgang når en brukerkonto synkroniseres med Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="eff88-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

