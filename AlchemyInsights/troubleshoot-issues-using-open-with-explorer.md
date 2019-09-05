---
title: Feilsøke problemer med åpne med Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742742"
---
# <a name="fix-problems-with-open-with-explorer"></a>Løs problemer med åpne med Explorer

Løs vanlige problemer med å åpne et dokumentbibliotek i SharePoint eller OneDrive ved hjelp av kommandoen **Åpne med Explorer** : 
  
- Bruk Internet Explorer 10 eller 11 for Internet Explorer. **Åpne med Explorer** er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre. **Åpne med Explorer** er deaktivert i alle nettlesere unntatt Internet Explorer. 
    
- **Åpne med Explorer** er ikke tilgjengelig i den moderne opplevelsen for SharePoint-biblioteker. Bruk **visning i Filutforsker** i stedet. Velg **Vis alternativer** \> **-visning i Filutforsker**. Utsikt inne arkiv utforske er ikke forenlig med Microsoft kant, Google Chrome, gi avskjed og andre. **Visning i Filutforsker** i bare tilgjengelig i Internet Explorer. 
    
- Kontroller at WebClient-tjenesten kjører. Skriv Kjør i søkeboksen i Windows, velg Kjør skrivebordsprogrammet, Skriv inn Services. msc, og trykk deretter ENTER. Bla ned til WebClient-tjenesten, og kontroller at **status** -kolonnen viser "running". Hvis den ikke gjør det, dobbeltklikker du tjenesten, klikker **Start**, og deretter klikker du **OK**. (Du må kanskje først aktivere tjenesten ved å velge enten **manuell** eller **automatisk** i boksen **Oppstartstype** .) 
    
> [!NOTE]
> Det er nyttig å åpne et bibliotek i Filutforsker hvis du må kopiere eller flytte flere filer og mapper én gang, men hvis du vil arbeide regelmessig i biblioteket, anbefaler vi at du synkroniserer det. Hvis du vil feilsøke problemer som åpnes i Filutforsker, kan du se [Åpne i Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Hvis du vil ha informasjon om hvordan du konfigurerer synkronisering, kan [du se synkronisere SharePoint-filer med den nye OneDrive Sync-klienten](https://go.microsoft.com/fwlink/?linkid=871666).
  
Se artikkelen [hvordan du bruker kommandoen "åpne med Explorer" til å feilsøke problemer i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for mer informasjon. 
  

