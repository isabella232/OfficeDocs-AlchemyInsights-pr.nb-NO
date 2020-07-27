---
title: Omgå aktiveringslås på overvåkede iOS-enheter med Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424218"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Omgå aktiveringslås på overvåkede iOS-enheter med Intune

Muligheten til å omgå aktiveringslåsen på iOS-enheter gjør det enklere å gjenopprette fra scenariet der en bruker aktiverer aktiveringslås på en bedriftsenhet, og forlater deretter selskapet.

Forutsetninger for å omgå en aktiveringslås inkluderer:

- En enhet er som er "overvåket".
- Aktiveringslåsen er aktivert ved hjelp av policyen for begrensning av iOS-enhet i Intune.

I tillegg, når du omgår en aktiveringslås, bør du:

- Fysisk besitte enheten blir tørket.
- Kopier koden før du utsteder slettingen.

**Merk:** Tørkkoden skiller ikke mellom store og små bokstaver, så "-" tegnene er ikke nødvendig.

Hvis du vil ha mer informasjon, kan du se [Omgå aktiveringslås på overvåkede iOS-enheter med Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**SPØRSMÅL OG SVAR**

Spørsmål: **Jeg utstedte en ekstern handling for å fjerne firmadata fra en enhet, og nå sitter det fast i en ventende tilstand.**

Svar: For at en ekstern handling skal kunne fullføres, må den målrettede enheten være tilkoblet og sunn. I følgende situasjoner forblir den eksterne handlingen i ventende tilstand i 30 dager, eller til enheten erkjenner kommandoen når enheten:

- Har ikke tilkobling.
- Mister sin lederstatus med Intune.

Hvis du tror at en enhet ikke lenger sjekker inn, og at den ikke fjerner firmadata, velger du Slett. Hvis du sletter enhetens post slik at den ikke lenger vises i Intune-listen over enheter. For at enheten skal bli aktiv igjen, må brukeren registrere enheten på nytt.

Spørsmål: **Hvorfor er visse eksterne handlinger ikke tilgjengelige for meg å bruke?**

Svar: Ikke alle plattformer støtter alle handlinger for eksterne enheter. Følgende eksterne handlinger er plattformspesifikke.

- Bypass aktiveringslås (bare iOS)
- Frisk start (bare Windows)
- Tapt modus (bare iOS)
- Finn enhet (bare iOS)
- Start på nytt (bare Windows)

Hvis du vil ha mer informasjon om hver handling, kan du se [Tilgjengelige enhetshandlinger](https://docs.microsoft.com/intune/device-management#available-device-actions).