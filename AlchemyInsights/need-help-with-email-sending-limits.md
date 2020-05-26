---
title: Trenger du hjelp med e-postsendingsgrenser?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357868"
---
# <a name="need-help-with-email-sending-limits"></a>Trenger du hjelp med e-postsendingsgrenser?

Nedenfor er **by-design sende grenser** håndheves i tjenesten. Mer informasjon om disse grensene er dokumentert [her](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).

- For å motvirke levering av uønskede massemeldinger, gjelder vi per bruker **mottaker sats grenser for alle utgående og interne meldinger**. På tvers av alle SKU-er er denne grensen **10 000 mottakere per dag**.  Kunder som trenger å sende legitim masse kommersiell e-post (for eksempel kundenyhetsbrev) bør bruke tredjepartsleverandører som spesialiserer seg på disse tjenestene.
    - **Merk:** Når mottakerhastighetsgrensen er nådd, kan ikke meldinger sendes fra postboksen før antall mottakere som ble sendt meldinger i løpet av de siste 24 timene faller under grensen. Brukeren vil ikke kunne sende meldinger før det punktet.
- Meldingshastighetsgrense på **30 meldinger per minutt** brukes på tvers av alle SKU-er. Dette bestemmer hvor mange meldinger en bruker kan sende fra Exchange Online-kontoen innen en angitt periode.
- Maksimalt antall mottakere som er tillatt i feltene **Til, Kopi og Blindkopi** for én enkelt e-postmelding på tvers av alle SKU-er, er **1000 mottakere**. Hvis du vil tilpasse denne grensen, kan du gå [hit](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).
