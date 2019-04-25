---
title: Feilsøke problemer med å bruke åpne med Explorer
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
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390616"
---
# <a name="fix-problems-with-open-with-explorer"></a>Løs problemer med åpne med Explorer

Løs vanlige problemer med å åpne et dokumentbibliotek i SharePoint eller OneDrive ved hjelp av kommandoen **Åpne med Explorer** : 
  
- Bruke Internet Explorer 10 eller 11 for Internet Explorer. **Åpne med Explorer** er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre. **Åpne med Explorer** er deaktivert i alle lesere bortsett fra Internet Explorer. 
    
- **Åpne med Explorer** er ikke tilgjengelig i den moderne opplevelsen for SharePoint-biblioteker. Bruk **visningen i File Explorer** i stedet. Velg **Alternativer for** \> **visning i Filutforsker**. Vis i File Explorer, er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre. **Vis i Filutforsker** i bare tilgjengelig i Internet Explorer. 
    
- Kontroller at WebClient-tjenesten kjører. I Windows søk-boksen, Skriv inn run, velger Kjør stasjonær programmet, Skriv inn services.msc og trykk deretter Enter. Rull ned til WebClient-tjenesten, og kontroller at **Status** -kolonnen viser "Som kjører." Hvis ikke, Dobbeltklikk tjenesten, klikk **Start**, og klikk deretter **OK**. (Du må kanskje først aktivere tjenesten ved å velge enten **Manuell** eller **automatisk** i boksen **Oppstartstype** .) 
    
> [!NOTE]
> Åpne et bibliotek i Filutforsker er nyttig hvis du skal kopiere eller flytte flere filer og mapper når, men hvis du vil arbeide regelmessig i biblioteket, anbefaler vi synkroniserer den. Hvis du vil feilsøke problemer med å åpne i File Explorer, kan du se [åpen i Explorer](https://go.microsoft.com/fwlink/?linkid=871665). For informasjon om hvordan du definerer synkronisering, kan du se [Synkroniser SharePoint-filer med den nye OneDrive sync-klienten](https://go.microsoft.com/fwlink/?linkid=871666).
  
Se [hvordan du bruker kommandoen "Åpne med Explorer" til å feilsøke problemer i SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) -artikkelen for mer informasjon. 
  

