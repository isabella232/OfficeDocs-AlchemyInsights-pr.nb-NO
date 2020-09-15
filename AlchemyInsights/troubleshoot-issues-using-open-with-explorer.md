---
title: Feilsøke problemer ved bruk av åpne med Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659067"
---
# <a name="fix-problems-with-open-with-explorer"></a>Løse problemer med åpne med Explorer

Løse vanlige problemer med å åpne et dokument bibliotek i SharePoint eller OneDrive ved hjelp av kommandoen **Åpne med Explorer** : 
  
- Bruk Internet Explorer 10 eller Internet Explorer 11. **Åpne med Explorer** er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre. **Åpne med Explorer** er deaktivert i alle nett lesere bortsett fra Internet Explorer. 
    
- **Åpne med Explorer** er ikke tilgjengelig i moderne opplevelse for SharePoint-biblioteker. Bruk **visning i fil Utforsker** i stedet. Velg **Vis alternativer** - \> **visning i fil Utforsker**. Vis i fil Utforsker er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre. **Vis bare i fil Utforsker** i tilgjengelig i Internet Explorer. 
    
- Kontroller at WebClient-tjenesten kjører. Skriv inn Kjør i Windows Search-boksen, velg Kjør skrive bords-appen, Skriv inn Services. msc, og trykk deretter ENTER. Rull ned til WebClient-tjenesten, og kontroller at **status** -kolonnen viser «kjører». Hvis den ikke gjør det, dobbelt klikker du tjenesten, klikker **Start**og deretter **OK**. (Du må kanskje først aktivere tjenesten ved å velge enten **manuell** eller **automatisk** i boksen **oppstarts type** .) 
    
> [!NOTE]
> Det er praktisk å åpne et bibliotek i fil Utforsker hvis du trenger å kopiere eller flytte flere filer og mapper én gang, men hvis du vil arbeide regelmessig i biblioteket, anbefaler vi at du synkroniserer det. Hvis du vil feilsøke problemer med å åpne i fil Utforsker, kan du se [Åpne i Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Hvis du vil ha informasjon om hvordan du konfigurerer synkronisering, kan du se [synkronisere SharePoint-filer med den nye synkroniserings klienten for OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).
  
Se artikkelen [Slik bruker du kommandoen «åpne med Explorer» til å feilsøke problemer i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for mer informasjon. 
  

