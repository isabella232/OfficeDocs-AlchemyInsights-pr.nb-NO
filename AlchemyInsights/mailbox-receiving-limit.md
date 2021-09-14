---
title: Håndhevelse av grense for postboksmottak
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/31/2021
ms.locfileid: "59316040"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Håndhevelse av grense for postboksmottak

Microsoft har nylig begynt å håndheve terskelen per postboks på 3600 meldinger per time. Hvis du vil ha mer informasjon, [kan du Exchange Online begrensninger](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits). Microsoft 365 postbokser som mottar over 3600 meldinger i løpet av en time, er begrensning i de neste 60 minuttene. 

I tillegg brukes grensen for avsenderpar (SRP) som blokkerer meldinger som mottas av en Microsoft 365 postboks fra en bestemt avsender. Hvis én enkelt avsender sender over 33 % av den totale terskelen eller 1200 meldinger per rullende time til en bestemt mottaker, starter SRP-grensen, og postboksen godtar ikke lenger meldinger fra denne avsenderen. Vær oppmerksom på at:

- Denne grensen gjelder for e-postmeldinger som er mottatt fra andre leiere, lokale avsendere eller Internett-avsendere.
- E-postlevering til postboksen er blokkert i de neste 60 minuttene. 
- Avsendere til disse postboksene mottar en rapport om manglende levering (5.2.121 eller 5.2.122) som sier at postboksen har overskredet den maksimale leveringsgrensen. Intra-tenant (e-post innenfor samme tenant) fortsetter å bli levert.
- Når SRP-grensen brukes, fortsetter den mottakende postboksen å godta meldinger fra andre avsendere.

Administratorer kan overvåke gjeldende postboksaktivitet ved å få tilgang til en ny rapport og innsikt i administrasjonssenteret Exchange kalt Postbokser som overskrider mottaksgrenser. Innsikten vises bare hvis en leier har uaksepterende postbokser, mens rapporten alltid vises i instrumentbordet, men er tom med mindre en leier har nærmet seg postbokser.

Hvis du vil ha mer informasjon om mottaksgrenser for innsikt, kan du se [Postbokser som overskrider mottaksgrenser, innsikt i den nye EAC](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights).

Hvis du vil ha mer informasjon om rapporten over mottaksgrenser, kan du se Postbokser som overskrider rapporten over mottaksgrenser [i den nye EAC](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report).