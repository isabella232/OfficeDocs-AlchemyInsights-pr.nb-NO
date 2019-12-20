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
ms.openlocfilehash: 46b23f97c2e682258224dc95e7a76b1201991828
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796267"
---
# <a name="troubleshooting-audio-problems-in-windows-10"></a>Feilsøke lydproblemer i Windows 10

**Kjøre feilsøking for lyd**

Feilsøking for lyd kan være i stand til å løse lyd problemene automatisk: 

1. Velg **Start**, Skriv **feilsøking**, og velg deretter **Feilsøk** fra listen over resultater. 
2. Velg **å spille av lyd** > **Kjør feilsøkingsprogrammet**.

**Kontroller kabler, volum, høyttalere og hodetelefoner**

- Kontroller tilkoblingene til høyttalerne og hodetelefonene for løse kabler, og kontroller at de er koblet til riktig kontakt.
- Kontroller strøm-og volumnivået, og prøv å slå alle volumkontrollene opp.
- Noen høyttalere og apper har egne volumkontroller, og du må kanskje kontrollere dem for å sikre at de er på riktig nivå.
- Prøv å koble til med en annen USB-port.
- **Merk:** Husk at høyttalerne kanskje ikke fungerer når hodetelefonene er plugget inn.

**Kontroller Enhetsbehandling**

Slik kontrollerer du at driverne er oppdatert:

- Velg **Start**, Skriv inn **Enhetsbehandling**, og velg deretter **Enhetsbehandling** fra listen over resultater.

2. Under **lyd-, video-og spillkontrollere**velger du lydkortet, åpner det, velger **driver** -fanen og velger **Oppdater driver**. 

**Merk:** Hvis Windows ikke finner en ny driver, kan du se etter en på enhetsprodusentens webområde og følge instruksjonene deres.

**Installer driveren på nytt**

Hvis du ikke kan oppdatere via Enhetsbehandling eller finne en ny driver på produsentens webområde, kan du prøve disse trinnene: 

1. I Enhetsbehandling høyreklikker du (eller trykker og holder) lyddriveren, og velger **Avinstaller**. Start enheten på nytt, og Windows prøver å installere driveren på nytt.

2. Hvis det ikke fungerer å installere driveren på nytt, kan du prøve å bruke den generiske lyddriveren som følger med Windows. I Enhetsbehandling høyreklikker du (eller trykker og holder) lyddriveren > **oppdatere driverprogramvare** > **Søk på datamaskinen etter driverprogramvare** > **La meg velge fra en liste over enhetsdrivere på datamaskinen**, velge **High Definition Audio-enhet**, velge **neste**og følge instruksjonene for å installere den.

**Angi standard enhet**

Hvis du kobler til en lydenhet ved hjelp av USB eller HDMI, må du kanskje angi denne enheten som standard: 

1. Velg **Start**, Skriv inn **lyd**, og velg deretter **lyd** eller **endre system lyder** fra resultatlisten.

2. Velg en enhet i kategorien **avspilling** , velg **Angi standard**, og velg deretter **OK**.

