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
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554342"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Når synkroniseres profil endringene til SharePoint-brukerprofilprogrammet?

SharePoint Online bruker tidtakerjobben for import av Active Directory (AD import) til å importere brukere og grupper til brukerprofilprogrammet. 
  
1. AD import synkroniserer endringer fra SharePoint Online Directory store til brukerprofilprogrammet. Disse endringene behandles i partier.
    
2. Tidtakerjobben kjøres til endringene er synkronisert.
    
> [!NOTE]
> Tiden det tar å kjøre jobben, avhenger av hvor mange endringer som skal utføres. Et stort antall endringer tar lengre tid. Service nivå avtalen (SLA) angir at en endring til en bruker i SharePoint Online Directory vil bli reflektert i brukerprofilprogrammet i 24 timer. 
  
[Mer informasjon om synkronisering av brukerprofiler i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

