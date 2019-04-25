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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Når Min profil endringer synkroniseres til brukerprofilprogrammet til SharePoint?

SharePoint Online bruker Active Directory-Import-tidtakerjobben (AD-Import) til å importere brukere og grupper til brukerprofilprogrammet. 
  
1. AD-Import synkroniserer endringer fra SharePoint Online Directory-butikken til brukerprofilprogrammet. Disse endringene er behandlet i kladder.
    
2. Tidtakerjobben kjøres til endringene er synkronisert.
    
> [!NOTE]
> Tiden det tar å kjøre jobben, avhengig av hvor mange endringer til å behandle. Et stort antall endringer tar lengre tid. Den Service tjenestenivåavtale (SLA) sier at en endring til en bruker i SharePoint Online Directory gjenspeiles i brukerprofilprogrammet i 24 timer. 
  
[Mer informasjon om brukerprofilsynkronisering i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

