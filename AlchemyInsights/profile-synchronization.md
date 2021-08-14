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
ms.openlocfilehash: b223bad66fb7cc6d1d7c0a2b3ccc7a081c061b4974060dbcafec84dfb24eb782
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923653"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Når synkroniseres profilen min til SharePoint brukerprofilprogrammet?

SharePoint Online bruker tidtakerjobben Active Directory Import (AD Import) til å importere brukere og grupper til brukerprofilprogrammet. 
  
1. AD Import synkroniserer endringer fra SharePoint Online Directory Store til brukerprofilprogrammet. Disse endringene behandles i grupper.
    
2. Tidtakerjobben kjører til endringene er synkronisert.
    
> [!NOTE]
> Hvor lang tid det tar å kjøre jobben, avhenger av antall endringer som skal behandles. Et stort antall endringer tar lengre tid. Tjenestenivåavtalen (SLA) sier at en endring av en bruker i SharePoint Online Directory gjenspeiles i brukerprofilprogrammet om 24 timer. 
  
[Mer informasjon om brukerprofilsynkronisering SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

