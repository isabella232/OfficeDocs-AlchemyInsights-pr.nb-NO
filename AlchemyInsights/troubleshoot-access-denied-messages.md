---
title: Feilsøking i forbindelse med nektet tilgang
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 05d12aee49b449e8a29e84021b41298fb9983859
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050714"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="fdd8f-102">Feilsøking i forbindelse med nektet tilgang</span><span class="sxs-lookup"><span data-stu-id="fdd8f-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="fdd8f-103">Hvis noen fikk en "ingen tilgang"-melding til en delt mappe i SharePoint, kan administratoren for områdesamlingen har aktivert låsing av brukertillatelsen begrenset tilgang til brukeren.</span><span class="sxs-lookup"><span data-stu-id="fdd8f-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="fdd8f-104">Slik slår du av denne:</span><span class="sxs-lookup"><span data-stu-id="fdd8f-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="fdd8f-105">Bla til området, klikker du innstillinger-ikonet, og klikk deretter **Innstillinger for webområde**.</span><span class="sxs-lookup"><span data-stu-id="fdd8f-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="fdd8f-106">Klikk **funksjoner for områdesamling**under **administrasjon av områdesamling**.</span><span class="sxs-lookup"><span data-stu-id="fdd8f-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="fdd8f-107">Klikk **Deaktiver**ved siden av **låsemodus for begrenset tilgang til bruker tillatelse**.</span><span class="sxs-lookup"><span data-stu-id="fdd8f-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="fdd8f-108">En Access denied-melding kan også forekomme for delte mapper hvis området er et publiseringsområde.</span><span class="sxs-lookup"><span data-stu-id="fdd8f-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="fdd8f-109">Hvis du vil ha informasjon, kan du se [tilgang nektet ved tilgang til en delt mappe](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="fdd8f-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="fdd8f-110">Hvis en person har en "ingen tilgang"-melding når du prøver å vise tilgangsforespørsler, må brukeren legges til som en administrator for områdesamling eller et medlem av gruppen eiere for området.</span><span class="sxs-lookup"><span data-stu-id="fdd8f-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="fdd8f-111">Hvis du vil ha mer informasjon, se [tilgang nektet tilgang til listen over forespørsler](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="fdd8f-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="fdd8f-112">Hvis en bruker fikk en "ingen tilgang"-melding etter at de ble fjernet fra Active Directory lokalt og deretter lagt tilbake, kan du se [Ingen tilgang når en brukerkonto er synkronisert til Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="fdd8f-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

