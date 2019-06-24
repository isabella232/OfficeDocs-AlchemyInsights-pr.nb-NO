---
title: Rette opp feil i 0x8004de40 i OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133985"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Rette opp feil i 0x8004de40 i OneDrive

Hvis du får en 0x8004de40-feil i OneDrive:

- Start på nytt den berørte datamaskinen mens du er koblet til aktvi Directory-domene.
- Hvis en omstart ikke løser problemet, melde deg ut og bli med enheten fra Azure AD. 

**Merk**: du bør være på firmanettverket mens du utfører disse trinnene. Ikke Utfør denne fremgangsmåten når du ikke kan koble til din bedriftens infrastruktur (for eksempel mens du reiser). 

- Åpne en ledetekst. 
- For å åpne en ledetekst, klikk - **Start**, høyreklikk **ledetekst**, og deretter klikker du **Kjør som administrator**.
- Skriv *dsregcmd /leave* , og trykk **Enter**.
- Når operasjonen er fullført, skriver du inn *dsregcmd-/join* , og trykk **Enter**.
- Når det er fullført, lukker du ledeteksten.
- Start datamaskinen på nytt og logge på OneDrive.