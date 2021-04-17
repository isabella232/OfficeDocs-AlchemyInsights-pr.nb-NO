---
title: Feilsøke lydproblemer i Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833300"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Feilsøke lydproblemer i Windows 10

**Kjøre feilsøking for lyd**

1.  Åpne [feilsøkingsinnstillingene](ms-settings:troubleshoot).

2.  Velg **Spill av lyd** Kjør  >  **feilsøkingsprogrammet**.

**Angi standardenheten**

Hvis du kobler til en lydenhet ved hjelp av USB eller HDMI, må du kanskje angi denne enheten som standard:

1. Åpne **Start**  >  **lyd**, og velg deretter **Lyd** eller **Endre systemlyder** fra listen over resultater.

2.  Velg en **enhet** på Avspilling-fanen, velg **Angi standard**, og velg deretter **OK**.

**Kontroller kabler, volum, høyttalere og hodetelefoner**

1. Kontroller høyttaler- og hodetelefontilkoblingene for løse kabler, og kontroller at de er koblet til riktig kontakt.

2. Kontroller strøm- og volumnivåene, og prøv å skru opp alle volumkontrollene.

3. Noen høyttalere og apper har sine egne volumkontroller. Du må kanskje kontrollere alle for å sikre at de er på riktig nivå.

4. Prøv å koble til med en annen USB-port.

**Obs!** Husk at høyttalerne kanskje ikke fungerer når hodetelefonene er koblet til.

**Kontroller Enhetsbehandling**

Slik kontrollerer du at driverne er oppdatert:

1. Velg **Start**, skriv **inn Enhetsbehandling**, og velg deretter **Enhetsbehandling** fra listen over resultater.

2. Velg **lydkortet under Lyd-, video-** og spillkontrollere, åpne det, velg **Driver-fanen** og velg **Oppdater driver**.

**Obs!** Hvis Windows ikke finner en ny driver, kan du se etter en på nettstedet til enhetsprodusenten og følge instruksjonene deres.

**Installere driveren på nytt**

Hvis du ikke kan oppdatere via Enhetsbehandling eller finne en ny driver på produsentens nettsted, kan du prøve disse trinnene:

1. Høyreklikk (eller trykk og hold) lyddriveren i **Enhetsbehandling,** og velg Avinstaller . Start enheten på nytt, så prøver Windows å installere driveren på nytt.

2. Hvis det ikke fungerer å installere driveren på nytt, kan du prøve å bruke den generiske lyddriveren som følger med Windows. Høyreklikk (eller trykk og hold) lyddriveren i Enhetsbehandling > Oppdater driverprogramvaren Bla gjennom datamaskinen for driverprogramvaren La meg velge fra en liste over enhetsdrivere på datamaskinen, velg  >    >    **Hd-lydenhet,** velg Neste , og følg instruksjonene for å installere den.
