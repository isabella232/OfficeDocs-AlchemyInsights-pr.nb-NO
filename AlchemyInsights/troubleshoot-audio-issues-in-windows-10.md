---
title: Feilsøke lydproblemer i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: f51fd233db5ae068e719f1cf3bc94a0dac82444f
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265025"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Feilsøke lydproblemer i Windows 10

**Kjøre feilsøking for lyd**

1.  Åpne [feilsøkingsinnstillingene](ms-settings:troubleshoot).

2.  Velg **Spille av lyd** > **Kjør feilsøkingsprogrammet**.

**Angi standardenheten**

Hvis du kobler til en lydenhet ved hjelp av USB eller HDMI, må du kanskje angi enheten som standard:

1. Åpne **Start** > **lyd**, og velg deretter **Lyd** eller **Endre systemlyder** fra listen over resultater.

2.  Velg en enhet i kategorien **Avspilling,** velg **Angi standard**, og velg deretter **OK**.

**Kontroller kabler, volum, høyttalere og hodetelefoner**

1. Kontroller høyttaler- og hodetelefontilkoblingene for løse kabler, og kontroller at de er koblet til riktig kontakt.

2. Kontroller strøm- og volumnivåene, og prøv å skru opp alle volumkontrollene.

3. Noen høyttalere og apper har sine egne volumkontroller. du må kanskje sjekke dem alle for å sikre at de er på riktig nivå.

4. Prøv å koble til ved hjelp av en annen USB-port.

**Merk:** Husk at høyttalerne kanskje ikke fungerer når hodetelefoner er koblet til.

**Sjekk Enhetsbehandling**

Slik kontrollerer du at driverne er oppdatert:

1. Velg **Start**, skriv inn **Enhetsbehandling**, og velg deretter **Enhetsbehandling** fra listen over resultater.

2. Velg lydkortet **under Lyd-, video- og spillkontrollere,** åpne det, velg **Driver-fanen** og velg **Oppdater driver**.

**Merk:** Hvis Windows ikke finner en ny driver, kan du se etter en på enhetsprodusentens nettsted og følge instruksjonene.

**Installere driveren på nytt**

Hvis du ikke kan oppdatere via Enhetsbehandling eller finne en ny driver på produsentens nettsted, kan du prøve disse trinnene:

1. Høyreklikk (eller trykk og hold) lyddriveren i Enhetsbehandling, og velg **Avinstaller**. Start enheten på nytt, så prøver Windows å installere driveren på nytt.

2. Hvis det ikke fungerer å installere driveren på nytt, kan du prøve å bruke den generiske lyddriveren som følger med Windows. I Enhetsbehandling høyreklikker du (eller trykker og holder) lyddriveren > **Oppdater driverprogramvare** > **Bla gjennom datamaskinen etter driverprogramvare** > **La meg velge fra en liste over enhetsdrivere på datamaskinen min**, velg **HD Audio Device**, velg **Neste**, og følg instruksjonene for å installere den.
