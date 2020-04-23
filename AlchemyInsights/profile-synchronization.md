---
title: Profilsynkronisering
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768122"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="54310-102">Når synkroniseres profilen min til SharePoint-brukerprofilprogrammet?</span><span class="sxs-lookup"><span data-stu-id="54310-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="54310-103">SharePoint Online bruker tidtakerjobben for Active Directory-import (AD-import) til å importere brukere og grupper til brukerprofilprogrammet.</span><span class="sxs-lookup"><span data-stu-id="54310-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="54310-104">AD Import synkroniserer endringer fra SharePoint Online Directory Store til brukerprofilprogrammet.</span><span class="sxs-lookup"><span data-stu-id="54310-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="54310-105">Disse endringene behandles i grupper.</span><span class="sxs-lookup"><span data-stu-id="54310-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="54310-106">Tidtakerjobben kjører til endringene er synkronisert.</span><span class="sxs-lookup"><span data-stu-id="54310-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="54310-107">Tiden det tar jobben å kjøre, avhenger av antall endringer som skal behandles.</span><span class="sxs-lookup"><span data-stu-id="54310-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="54310-108">Et stort antall endringer tar lengre tid.</span><span class="sxs-lookup"><span data-stu-id="54310-108">A large number of changes takes longer.</span></span> <span data-ttu-id="54310-109">Servicelevel-avtalen (Service Level Agreement) sier at en endring til en bruker i SharePoint Online-katalogen gjenspeiles i brukerprofilprogrammet om 24 timer.</span><span class="sxs-lookup"><span data-stu-id="54310-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="54310-110">Mer informasjon om synkronisering av brukerprofil i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="54310-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

