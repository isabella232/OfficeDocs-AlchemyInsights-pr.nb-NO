---
title: Kontrollsensorstatus for Defender-endepunkt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676342"
---
# <a name="defender-endpoint-check-sensor-status"></a>Kontrollsensorstatus for Defender-endepunkt

Flisen **Enheter med sensorproblemer** er plassert på instrumentbordet for sikkerhetsoperasjoner. Denne flisen gir informasjon om den enkelte enhetens mulighet til å gi sensordata og kommunisere med Defender for endpoint-tjenesten. Den rapporterer hvor mange enheter som krever oppmerksomhet og hjelper deg med å identifisere problematiske enheter og iverksette tiltak for å løse kjente problemer.

To statusindikatorer på flisen gir informasjon om antall enheter som ikke rapporterer riktig til tjenesten:

- **Feilkonfigurert** Enheter som kanskje delvis rapporterer sensordata til Defender for Endpoint-tjenesten, og som kan ha konfigurasjonsfeil som må rettes opp.
- **Inaktiv** Enheter som har sluttet å rapportere til Defender for endepunkttjenesten i mer enn sju dager den siste måneden.

Når du klikker en av gruppene, dirigerer du til Enheter-listen, filtrert i henhold til valgene dine. I Enheter-listen kan du filtrere tilstandsstatuslisten etter følgende status:

- **Aktiv** Enheter som aktivt rapporterer til Defender for endepunkttjenesten.
- **Feilkonfigurert** Enheter som delvis rapporterer sensordata til Defender for endpoint-tjenesten, men som har konfigurasjonsfeil som må rettes opp. Feilkonfigurerte enheter kan ha enten én eller en kombinasjon av følgende problemer:

    - Ingen sensordata – Enheter har sluttet å sende sensordata. Begrensede varsler kan utløses fra enheten.
    - Nedsatt kommunikasjon – Muligheten til å kommunisere med enheten er nedsatt. Sending av filer for dyp analyse, blokkering av filer, isolering av enhet fra nettverket og andre handlinger som krever kommunikasjon med enheten, fungerer kanskje ikke.
- **Inaktiv** Enheter som har sluttet å rapportere til Defender for endepunkttjenesten.

Du kan laste ned hele listen i CSV-format ved hjelp av Eksporter-funksjonen.

Hvis du vil ha mer informasjon, kan du se Kontrollere tilstanden til [sensoren i Microsoft Defender for endepunkt](/microsoft-365/security/defender-endpoint/check-sensor-status).

Hvis du vil ha mer informasjon om hva som førte til at en enhet var inaktiv eller feilkonfigurert, kan du se Reparere usunne sensorer i [Microsoft Defender for endepunkt](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).
