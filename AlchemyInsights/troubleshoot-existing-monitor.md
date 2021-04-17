---
title: Feilsøke eksisterende skjerm
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824588"
---
# <a name="troubleshoot-an-existing-monitor"></a>Feilsøke en eksisterende skjerm

Prøv disse løsningene for å feilsøke en skjerm. 

**Oppdater skjermens skjerm:**

Trykk følgende taster samtidig: Windows-tast + CTRL + SKIFT + B. Dette vil oppdatere kommunikasjonen med grafikkdriveren. Skjermene blinker et øyeblikk og kommer tilbake etter noen sekunder.

**Feilsøke maskinvare for skjerm:**

1. Koble kabelen som kobler PC-en til skjermen, og koble den til igjen.
2. Koble alle ikke-essensielle enheter fra PC-en (for eksempel adaptere eller dokkingstasjoner).

**Hvis du nylig har installert en oppdatering på PC-en, kan du rulle tilbake skjermdriveren:**

1. Velg **Start**, skriv **inn enhetsbehandling**, og velg **Enhetsbehandling** fra resultatene.
2. Utvid **delen Skjermkort,** høyreklikk skjermkortet, og velg **Egenskaper**.
3. Gå til **Driver-fanen,** og velg **Rull tilbake driver**. <br>
Obs! Hvis dette ikke er tilgjengelig eller  nedtonet, velger du Nei fra alternativene nedenfor for å gå til neste trinn.
4. Du må kanskje starte PC-en på nytt før disse endringene trer i kraft.

**Avinstaller skjermdriveren og installer den på nytt:**

1. Velg **Start**, skriv **inn enhetsbehandling**, og velg **Enhetsbehandling** fra resultatene.
2. Utvid **Delen Skjermkort,** høyreklikk skjermkortet, og velg **Avinstaller enhet**. 
3. Velg boksen ved siden av **Slett driverprogramvaren for denne enheten,** og velg **Avinstaller**.<br>
Obs! Du kan bli bedt om å starte datamaskinen på nytt på dette stadiet. Pass på å skrive ned de gjenværende instruksjonene før du starter på nytt.
4. Åpne Enhetsbehandling på nytt.
5. Utvid **delen Skjermkort,** høyreklikk på skjermkortet, og velg **Oppdater driver**.
6. Velg **Søk automatisk etter oppdateringsdriverprogramvare,** og følg installasjonsinstruksjonene.