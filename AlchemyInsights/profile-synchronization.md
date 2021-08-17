---
title: Profilsynkronisering
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320718"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Når synkroniseres profilen min til SharePoint brukerprofilprogrammet?

SharePoint Online bruker tidtakerjobben Active Directory Import (AD Import) til å importere brukere og grupper til brukerprofilprogrammet. 
  
1. AD Import synkroniserer endringer fra SharePoint Online Directory Store til brukerprofilprogrammet. Disse endringene behandles i grupper.
    
2. Tidtakerjobben kjører til endringene er synkronisert.
    
**Obs!** Tiden det tar å kjøre jobben, avhenger av antall endringer som skal behandles. Et stort antall endringer tar lengre tid. Tjenestenivåavtalen (SLA) sier at en endring av en bruker i SharePoint Online Directory gjenspeiles i brukerprofilprogrammet om 24 timer. 
  
[Mer informasjon om brukerprofilsynkronisering i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

