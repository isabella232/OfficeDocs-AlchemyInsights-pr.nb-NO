---
title: Feilsøke problemer ved bruk av Åpne med Explorer
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
ms.openlocfilehash: 0cbcfb506295d5732f7109be7a103bbdef530a529c7408c6d9d45a7b38a89915
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048165"
---
# <a name="fix-problems-with-open-with-explorer"></a>Løse problemer med Åpne med Explorer

Løse vanlige problemer med å åpne et dokumentbibliotek i SharePoint eller OneDrive ved hjelp av kommandoen Åpne **med Explorer:** 
  
- Bruk Internet Explorer 10 eller Internet Explorer 11. **Åpne med Explorer** er ikke kompatibelt med Microsoft Edge, Google Chrome, Firefox og andre. **Åpne med Explorer** er deaktivert i alle nettlesere unntatt Internet Explorer. 
    
- **Åpne med Explorer** er ikke tilgjengelig i den moderne opplevelsen for SharePoint biblioteker. Bruk **Visning i Filutforsker i** stedet. Velg **Visningsalternativer** \> **Vis i Filutforsker**. Visning i Filutforsker er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre. **Vis i Filutforsker i** bare tilgjengelig i Internet Explorer. 
    
- Kontroller at WebClient-tjenesten kjører. Skriv inn Windows i søkeboksen, velg Kjør skrivebordsprogrammet, skriv inn services.msc, og trykk deretter ENTER. Rull ned til WebClient-tjenesten, og kontroller at **Status-kolonnen** viser «Kjører». Hvis den ikke gjør det, dobbeltklikker du tjenesten, klikker **Start** og deretter **OK**. (Du må kanskje først aktivere tjenesten ved å velge Enten **Manuell** eller **Automatisk** i **Oppstartstype-boksen.)** 
    
> [!NOTE]
> Det er praktisk å åpne et bibliotek i Filutforsker hvis du trenger å kopiere eller flytte flere filer og mapper én gang, men hvis du vil arbeide regelmessig i biblioteket, anbefaler vi at du synkroniserer det. Hvis du vil feilsøke problemer med å åpne i Filutforsker, kan [du se Åpne i Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Hvis du vil ha informasjon om hvordan du konfigurerer [synkronisering, kan du se Synkronisere SharePoint filer med den nye OneDrive-synkronisering klienten](https://go.microsoft.com/fwlink/?linkid=871666).
  
Se artikkelen Slik bruker du kommandoen Åpne med [Explorer til](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) å feilsøke problemer i SharePoint Online hvis du vil ha mer informasjon. 
  

