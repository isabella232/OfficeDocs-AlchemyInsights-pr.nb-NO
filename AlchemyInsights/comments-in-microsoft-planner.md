---
title: Kommentarer i Microsoft Planner
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001717"
- "3810"
ms.openlocfilehash: 0d87d8c9fafe49de02b9c0158144287c77339886cdb910e006296eac73a2c497
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995516"
---
# <a name="comments-in-microsoft-planner"></a>Kommentarer i Microsoft Planner

Kommentarer for oppgaver i en plan lagres i Exchange Online-postboksen til Microsoft 365-gruppen som er tilknyttet planen.  Når du publiserer en kommentar på en oppgave, sendes det et e-postvarsel til gruppeinnboksen, og du får tilsendt en e-post for hver nye kommentar som publiseres på den aktuelle oppgaven.

Her er noen svar på vanlige problemer knyttet til kommentarer:

- **Brukere mottar ikke e-poster** – Kommentarer sendes til gruppeinnboksen til gruppen som planen tilhører. For at en bruker skal kunne motta gruppe-e-poster, må gruppen være konfigurert for å sende gruppesamtaler til medlemmenes innbokser.

- **Kommentarer lagres ikke** – Brukeren som legger til kommentaren har ikke tillatelse til å sende e-poster til Microsoft 365-gruppen. Les [Slik fungerer Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) for mer informasjon om dette scenarioet.

- Feilmeldingen **Du har ikke lenger tilgang** vises, eller **gjestebrukere kan ikke legge til kommentarer** – Det kan være at gjestebrukere som ikke kan sende e-poster til gruppeinnboksen ser denne meldingen. Du kan løse problemet ved å sørge for at gjestebrukeren har en gyldig e-postadresse.

- **Fjernede brukere mottar e-poster** – Hvis en bruker kommenterer på en oppgave før vedkommende blir fjernet fra planen, vil e-posttråden inkludere brukeren for hver kommentar som publiseres på oppgaven.

Hvis du vil ha mer detaljert informasjon om kommentarer med Microsoft Planner, kan du ta en titt på [slik fungerer Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) og [Kommentere på oppgaver i Microsoft Planner](https://support.microsoft.com/office/fd4aedde-7785-4cd0-96ee-122fbc9140e1).
