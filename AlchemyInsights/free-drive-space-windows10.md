---
title: Frigjøre diskplass i Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036591"
---
# <a name="free-up-drive-space-in-windows-10"></a>Frigjøre diskplass i Windows 10

Her er to alternativer for å frigjøre diskplass i Windows:

- Frigjør diskplass i Windows 10.
- Frigjør plass til Windows 10-oppdateringer med ekstern lagringsenhet.

Hvis du fremdeles har lite diskplass etter å ha brukt Diskopprydding, er det mulig at Temp-mappen raskt fylles opp med programfiler (APPX) som brukes av Microsoft Store. Hvis du vil løse dette problemet, tilbakestiller du Store, tømmer Store-bufferen og kjører deretter feilsøkingsprogrammet for Windows Update. Kontroller at Microsoft Store er lukket før du fortsetter med disse trinnene.

**Trinn 1: Tilbakestille Microsoft Store**

**Obs!** Dette sletter appdataene på enheten permanent, inkludert innstillingene og påloggingsdetaljene.

1. Velg **Start**  >  **Innstillinger-apper**  >    >  **apper & funksjoner**.

1. Finn og velg Microsoft Store i listen over apper.

1. Velg **Avanserte alternativer**.

1. Rull nedover, **og velg Tilbakestill**, og deretter **Bekreft tilbakestilling**.

**Trinn 2: Tøm hurtigbufferen for Microsoft Store**

1. Trykk Windows-logotasten + R for å åpne dialogboksen Kjør.

1. Skriv wsreset.exe, og velg **OK**.

1. Et tomt ledetekstvindu åpnes. Etter omtrent 10 sekunder lukkes vinduet, og Store åpnes automatisk.

**Trinn 3: Tilbakestille Windows Update**

1. Velg **Start innstillinger**  >  **Oppdater**&  >  **sikkerhetsfeilsøking**  >  .

1. Rull nedover og **velg Windows Update** fra listen, og velg Kjør **feilsøkingsprogrammet**.

1. Start datamaskinen på nytt, og kontroller om du fremdeles har problemet.

