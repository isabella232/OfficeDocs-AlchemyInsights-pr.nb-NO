---
title: Fix 0x8004de40 feil i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052046"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Fix 0x8004de40 feil i OneDrive

Hvis du får en 0x8004de40-feil med OneDrive:

- Gjenstarte det berørt computer stund koplet å din aktvi adresseliste domenen.
- Hvis en omstart ikke løser problemet, melde deg ut og bli med enheten fra Azure AD. 

**Merk**: du bør være på bedriftsnettverket mens du utfører disse trinnene. Ikke Utfør disse trinnene når du ikke kan koble til bedriftsinfrastrukturen (for eksempel mens du er på reise). 

- Åpne en hevet ledetekst. 
- Å åpen en opphøyet kommandere spørsmål, falle i staver- **starte**, rett-falle i staver **kommandere spørsmål**, og så falle **i staver løpe idet administrator**.
- Skriv inn *dsregcmd/Leave* og trykk **Enter**.
- Når du er ferdig, skriver du inn *dsregcmd/JOIN* og trykker **Enter**.
- Når du er ferdig, lukker du ledeteksten.
- Start datamaskinen på nytt, og Logg på OneDrive.