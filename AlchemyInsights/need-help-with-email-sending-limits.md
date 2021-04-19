---
title: Trenger du hjelp med sendingsgrenser for e-post?
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
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836288"
---
# <a name="need-help-with-email-sending-limits"></a>Trenger du hjelp med sendingsgrenser for e-post?

Nedenfor finner **du grensene for sending av by-design** som er håndhevet i tjenesten. Mer informasjon om disse grensene er [dokumentert her](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).

- Hvis du vil fraråde levering av uoppfordrede massemeldinger, bruker vi satsegrenser per bruker på alle **utgående og interne meldinger.** På tvers av alle SKUs er denne grensen **10 000 mottakere per dag.**  Kunder som trenger å sende legitime masseutsendelser av kommersiell e-post (for eksempel kundenyhetsbrev), bør bruke tredjepartsleverandører som er spesialister på disse tjenestene.
    - **Obs!** Når grensen for mottakerfrekvens er nådd, kan ikke meldinger sendes fra postboksen før antall mottakere som ble sendt meldinger i løpet av de siste 24 timene, faller under grensen. Brukeren kan ikke sende meldinger før dette tidspunktet.
- Grensen for meldingsfrekvens **på 30 meldinger per minutt** brukes på tvers av alle SKUs. Dette bestemmer hvor mange meldinger en bruker kan sende fra Exchange Online-kontoen i løpet av en angitt periode.
- Maksimalt antall mottakere som er tillatt i Feltene **Til,** Kopi og Blindkopi for én enkelt e-postmelding, på tvers av alle SKUs, er **1000 mottakere.** Hvis du vil tilpasse denne grensen, kan du [gå hit](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).
