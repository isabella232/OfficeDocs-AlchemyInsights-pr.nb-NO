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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Når synkroniseres profilen min til SharePoint-brukerprofilprogrammet?

SharePoint Online bruker tidtakerjobben for Active Directory-import (AD-import) til å importere brukere og grupper til brukerprofilprogrammet. 
  
1. AD Import synkroniserer endringer fra SharePoint Online Directory Store til brukerprofilprogrammet. Disse endringene behandles i grupper.
    
2. Tidtakerjobben kjører til endringene er synkronisert.
    
> [!NOTE]
> Tiden det tar jobben å kjøre, avhenger av antall endringer som skal behandles. Et stort antall endringer tar lengre tid. Servicelevel-avtalen (Service Level Agreement) sier at en endring til en bruker i SharePoint Online-katalogen gjenspeiles i brukerprofilprogrammet om 24 timer. 
  
[Mer informasjon om synkronisering av brukerprofil i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

