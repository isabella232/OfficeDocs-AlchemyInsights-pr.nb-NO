---
title: Feilsøke problemer ved hjelp av Åpne med Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759701"
---
# <a name="fix-problems-with-open-with-explorer"></a>Løse problemer med Åpne med Explorer

Løse vanlige problemer med å åpne et dokumentbibliotek i SharePoint eller OneDrive ved hjelp av kommandoen **Åpne med Explorer:** 
  
- Bruk Internet Explorer 10 eller Internet Explorer 11. **Åpne med Explorer** er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre. **Åpen med Explorer** er deaktivert i alle nettlesere unntatt Internet Explorer. 
    
- **Åpen med Explorer** er ikke tilgjengelig i den moderne opplevelsen for SharePoint-biblioteker. Bruk **vis i Filutforsker** i stedet. Velg **Vis alternativer** \> **Vis i Filutforsker**. Visning i Filutforsker er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre. **Vis i Filutforsker** på tilgjengelig bare i Internet Explorer. 
    
- Kontroller at WebClient-tjenesten kjører. Skriv inn kjør i Søkeboksen i Windows, velg Kjør skrivebord-appen, skriv inn services.msc, og trykk deretter Enter. Rull ned til WebClient-tjenesten, og kontroller at **Status-kolonnen** viser "Kjører". Hvis den ikke gjør det, dobbeltklikker du tjenesten, klikker **Start**, og deretter klikker du **OK**. (Du må kanskje aktivere tjenesten først ved å velge **manuell** eller **automatisk** i **oppstartstype-boksen.)** 
    
> [!NOTE]
> Det er nyttig å åpne et bibliotek i Filutforsker hvis du må kopiere eller flytte flere filer og mapper én gang, men hvis du vil arbeide regelmessig i biblioteket, anbefaler vi at du synkroniserer det. Hvis du vil feilsøke problemer med å åpne filutforsker, kan du se [Åpne i Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Hvis du vil ha informasjon om hvordan du konfigurerer synkronisering, kan du se [Synkronisere SharePoint-filer med den nye OneDrive-synkroniseringsklienten](https://go.microsoft.com/fwlink/?linkid=871666).
  
Se artikkelen [Slik bruker du kommandoen "Åpne med Explorer" til å feilsøke problemer i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) hvis du vil ha mer informasjon. 
  

