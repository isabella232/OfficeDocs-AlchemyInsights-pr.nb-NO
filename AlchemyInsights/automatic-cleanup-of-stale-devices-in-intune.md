---
title: Automatisk opprydding av foreldede enheter i Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555225"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Automatisk opprydding av foreldede enheter i Intune

Intune gjør det mulig for administratoren å konfigurere et tidsintervall mellom 90 og 270 dager, hvoretter foreldede enheter fjernes fra tjenesten. Denne innstillingen er organisasjonen bred og når aktivert trer i kraft umiddelbart. Alle enheter som ikke er sjekket inn på Intune-serveren i en periode som overskrider innstillingen, slettes permanent.

**Merk at** Bare MDM-enhetsobjekter er kvalifisert for denne oppryddingshandlingen. EAS er bare enhetsobjekter som er utelukket.

Hvis du vil ha mer informasjon om når en enhet blir kvalifisert for sletting basert på opprydningsinnstillingen for enheten og "tilstand":

Innstilling: **Slett enheter etter siste innsjekkingsdato: Ja (noe verdi (N) i angitte dager)**

- Basert på verdien (N) som er konfigurert i innstillingen, sletter Intune-tjenesten enheten i de angitte dagene etter at den sist ble kontrollert.

Innstilling: **Slett enheter etter siste innsjekkingsdato: Nei**

- 180 dager etter at enhetssertifikatet utløper og ikke fornyes, slettes enheten.

**Merk at** I begge tilfeller må enheten registreres i Intune. Registrering skjer under den første enhetskontrollen med Intune-tjenesten.

Hvis en enhet registrerer seg for å være på Intune, men ikke blir Intune registrert, slettes enheten 270 dager etter registrering. (90 dager for å merke enheten som tilbakekalt, og deretter ytterligere 180 dager til å slette posten.)

Det finnes for øyeblikket ingen mekanisme i Intune-konsollen for å opprette utløpsdatoen for enhetssertifiseringen for en gitt enhet.