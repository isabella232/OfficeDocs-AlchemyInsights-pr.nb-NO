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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Når blir profilen min synkronisert til bruker profil programmet for SharePoint?

SharePoint Online bruker tid taker jobben for Active Directory import (AD-import) til å importere brukere og grupper til bruker profil programmet. 
  
1. AD import synkroniserer endringer fra katalog butikken i SharePoint Online til bruker profil programmet. Disse endringene behandles i grupper.
    
2. Tid taker jobben kjører til endringene er synkronisert.
    
> [!NOTE]
> Tiden det tar å kjøre jobben, avhenger av antall endringer som skal behandles. Et stort antall endringer tar lenger tid. Tjeneste nivå avtalen angir at en endring i en bruker i SharePoint Online-katalogen vil bli gjen speilet i bruker profil programmet i 24 timer. 
  
[Mer informasjon om bruker profil synkronisering i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

