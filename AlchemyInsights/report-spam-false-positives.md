---
title: Vil du rapportere et falskt søppelpost-positivt til Microsoft?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396624"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Merkes ekte meldinger som søppelpost?

Det er frustrerende når en legitim e-postmelding havner i Søppelpost-mappen eller i karantene. Vurder disse vanligste årsakene til falske positiver:

**Overstyringer for leieren (mest vanlig)** Dette er fullstendig innenfor din kontroll for å utbedre.

Send meldingen på Microsoft 365 Defender for analyse av de påvirkende policyene og reglene; Informasjon om ny kanne er tilgjengelig i løpet av noen minutter.
Se gjennom eller endre policyene eller reglene etter hva som er aktuelt. 

**Overstyringer for sluttbrukere (vanlig)** Dette er fullstendig innenfor din kontroll for å utbedre. 

Send meldingen på Microsoft 365 Defender for analyse av de påvirkende policyene og reglene; Informasjon om ny kanne er tilgjengelig i løpet av noen minutter. 

Hvis en melding ble blokkert fordi den ble sendt fra en adresse i en brukers liste over blokkerte avsendere, inneholder overskriftene søppelpostfiltreringsdommen «SFV:BLK».

**Avsenderes e-postgodkjenning** Dette er delvis innenfor kontrollen for å utbedre.

Send meldingen for å analysere feil i avsenderens e-postgodkjenning på leveringstidspunktet. resultatene er tilgjengelige i løpet av en dag. 

Hvis du eier infrastrukturen for sending, kan du se gjennom hvordan du justerer den med SPF, DKIM og DMARC for å sikre at e-postsystemer for mål klarerer meldinger som sendes fra domenet. Alternativt kan du kontakte avsenderne for å løse DNS-konfigurasjonene.

**Microsoft-filtreringskjennelser** Dette er delvis innenfor kontrollen for å utbedre.

Send meldingen og rapporter meldingen som sikker. rescan results are available within a day. Bruk tillatelses-/blokkeringslisten for leieren når du er uenig i filtreringskjennelser i bestemte situasjoner. Du bør imidlertid ikke omgå Microsoft-filtreringskjennelser permanent. 

Hvis du vil ha mer informasjon, kan du se:

- La sluttbrukerne sende meldinger til Microsoft. Microsoft bruker disse innsendingene til å forbedre effektiviteten til e-postbeskyttelsesteknologier, og de vises i innsendingsrapporter som du kan bruke som en indikasjon på oppdatering av policyer. 

- Hvis du vil se en kort video om å sende inn meldinger til analyse, kan du [se Sende inn meldinger for analyse](https://go.microsoft.com/fwlink/?linkid=2166435).

- [Bruke administratorinnsending til å sende inn mistenkelig søppelpost, phish, nettadresser og filer til Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Administrere tillatelses-/blokkeringslisten for leieren](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Søppelposthoder i Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Beskyttelse mot utgående søppelpost i EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)