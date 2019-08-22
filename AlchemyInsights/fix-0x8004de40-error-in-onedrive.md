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
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525068"
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