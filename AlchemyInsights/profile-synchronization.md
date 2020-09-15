---
title: Profil synkronisering
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801778"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="a0d17-102">Når blir profilen min synkronisert til bruker profil programmet for SharePoint?</span><span class="sxs-lookup"><span data-stu-id="a0d17-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="a0d17-103">SharePoint Online bruker tid taker jobben for Active Directory import (AD-import) til å importere brukere og grupper til bruker profil programmet.</span><span class="sxs-lookup"><span data-stu-id="a0d17-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="a0d17-104">AD import synkroniserer endringer fra katalog butikken i SharePoint Online til bruker profil programmet.</span><span class="sxs-lookup"><span data-stu-id="a0d17-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="a0d17-105">Disse endringene behandles i grupper.</span><span class="sxs-lookup"><span data-stu-id="a0d17-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="a0d17-106">Tid taker jobben kjører til endringene er synkronisert.</span><span class="sxs-lookup"><span data-stu-id="a0d17-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="a0d17-107">Tiden det tar å kjøre jobben, avhenger av antall endringer som skal behandles.</span><span class="sxs-lookup"><span data-stu-id="a0d17-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="a0d17-108">Et stort antall endringer tar lenger tid.</span><span class="sxs-lookup"><span data-stu-id="a0d17-108">A large number of changes takes longer.</span></span> <span data-ttu-id="a0d17-109">Tjeneste nivå avtalen angir at en endring i en bruker i SharePoint Online-katalogen vil bli gjen speilet i bruker profil programmet i 24 timer.</span><span class="sxs-lookup"><span data-stu-id="a0d17-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="a0d17-110">Mer informasjon om bruker profil synkronisering i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a0d17-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

