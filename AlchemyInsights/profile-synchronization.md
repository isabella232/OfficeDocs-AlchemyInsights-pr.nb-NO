---
title: Profilsynkronisering
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371993"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="02714-102">Når Min profil endringer synkroniseres til brukerprofilprogrammet til SharePoint?</span><span class="sxs-lookup"><span data-stu-id="02714-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="02714-103">SharePoint Online bruker Active Directory-Import-tidtakerjobben (AD-Import) til å importere brukere og grupper til brukerprofilprogrammet.</span><span class="sxs-lookup"><span data-stu-id="02714-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="02714-104">AD-Import synkroniserer endringer fra SharePoint Online Directory-butikken til brukerprofilprogrammet.</span><span class="sxs-lookup"><span data-stu-id="02714-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="02714-105">Disse endringene er behandlet i kladder.</span><span class="sxs-lookup"><span data-stu-id="02714-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="02714-106">Tidtakerjobben kjøres til endringene er synkronisert.</span><span class="sxs-lookup"><span data-stu-id="02714-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="02714-107">Tiden det tar å kjøre jobben, avhengig av hvor mange endringer til å behandle.</span><span class="sxs-lookup"><span data-stu-id="02714-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="02714-108">Et stort antall endringer tar lengre tid.</span><span class="sxs-lookup"><span data-stu-id="02714-108">A large number of changes takes longer.</span></span> <span data-ttu-id="02714-109">Den Service tjenestenivåavtale (SLA) sier at en endring til en bruker i SharePoint Online Directory gjenspeiles i brukerprofilprogrammet i 24 timer.</span><span class="sxs-lookup"><span data-stu-id="02714-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="02714-110">Mer informasjon om brukerprofilsynkronisering i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="02714-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

