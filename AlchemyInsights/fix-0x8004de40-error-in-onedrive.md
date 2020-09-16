---
title: Løse 0x8004de40-feil i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745139"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Løse 0x8004de40-feil i OneDrive

Hvis du får en 0x8004de40-feil med OneDrive:

- Start den berørte data maskinen på nytt mens du er koblet til Acitve Directory-domenet.
- Hvis en omstart ikke løser problemet, kan du koble fra enheten og koble den til på nytt fra Azure AD. 

**Merk**: du bør være på bedrifts nettverket mens du utfører disse trinnene. Ikke Utfør denne Fremgangs måten når du ikke kan koble til infrastrukturen for bedriften (for eksempel mens du er på reise). 

- Åpne en hevet lede tekst. 
- Hvis du vil åpne en hevet lede tekst, klikker du- **Start**, høyre klikker lede **tekst**, og klikker deretter **Kjør som administrator**.
- Skriv inn *dsregcmd/Leave* , og trykk **Enter**.
- Når du er ferdig, skriver du inn *dsregcmd/JOIN* og trykker **Enter**.
- Når du er ferdig, lukker du lede teksten.
- Start data maskinen på nytt, og Logg på OneDrive.