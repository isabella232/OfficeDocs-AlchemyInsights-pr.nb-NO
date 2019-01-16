---
title: Feilsøking i forbindelse med tilgang til meldinger
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3973f5bf584343d3353e7389f22bc727827b5c35
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28303237"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="cb5dd-102">Feilsøking i forbindelse med tilgang til meldinger</span><span class="sxs-lookup"><span data-stu-id="cb5dd-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="cb5dd-p101">Hvis noen fikk meldingen "Ingen tilgang" til en delt mappe, administratoren for områdesamlingen kan du har aktivert "begrenset tilgang tillatelse lockdown brukermodus." Slik deaktiverer du dette:</span><span class="sxs-lookup"><span data-stu-id="cb5dd-p101">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode." To turn this off:</span></span> 
  
1. <span data-ttu-id="cb5dd-105">Gå til webområdet, klikker du ikonet og klikk deretter **Områdeinnstillinger**.</span><span class="sxs-lookup"><span data-stu-id="cb5dd-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="cb5dd-106">Under **Administrasjon av områdesamling**, klikker du **funksjoner i områdesamling**.</span><span class="sxs-lookup"><span data-stu-id="cb5dd-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="cb5dd-107">Ved siden av **låsing av modus for begrenset tilgang brukeren tillatelse**, klikker du **Deaktiver**.</span><span class="sxs-lookup"><span data-stu-id="cb5dd-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="cb5dd-p102">Feilmeldingen Ingen tilgang kan også oppstå for delte mapper hvis området er et publiseringsområde. For informasjon, kan du se [Tilgang når du åpner en delt mappe](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="cb5dd-p102">An Access Denied message can also occur for shared folders if the site is a publishing site. For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="cb5dd-p103">Hvis en noen fikk meldingen "Ingen tilgang" når du prøver å vise forespørsler om tilgang, må brukeren som skal legges til som en administrator eller medlem av gruppen eiere for området. For mer informasjon, kan du se [Tilgang til listen over forespørsler om tilgang](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="cb5dd-p103">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site. For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="cb5dd-112">Hvis en bruker har fått meldingen "Ingen tilgang" når de ble fjernet fra Active Directory på lokaler og deretter legges tilbake, kan du se [Tilgang når en brukerkonto som synkroniseres til Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="cb5dd-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

