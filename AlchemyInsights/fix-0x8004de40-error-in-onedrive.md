---
title: Løs 0x8004de40-feil i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716037"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Løs 0x8004de40-feil i OneDrive

Hvis du får en 0x8004de40-feil med OneDrive:

- Start den berørte datamaskinen på nytt mens den er koblet til Acitve Directory-domenet.
- Hvis en omstart ikke løser problemet, kan du slutte å bli med på enheten og bli med på nytt fra Azure AD. 

**Merk:** Du bør være på bedriftsnettverket mens du utfører disse trinnene. Ikke utfør disse trinnene når du ikke kan koble til bedriftens infrastruktur (for eksempel mens du reiser). 

- Åpne en hevet ledetekst. 
- Hvis du vil åpne en hevet ledetekst, klikker du - **Start**, høyreklikker **Ledetekst**, og deretter klikker du Kjør **som administrator**.
- Skriv *inn dsregcmd /leave,* og trykk **Enter**.
- Når du er ferdig, skriver du inn *dsregcmd /join* og trykker **Enter**.
- Når du er ferdig, lukker du ledeteksten.
- Start datamaskinen på nytt, og logg på OneDrive.