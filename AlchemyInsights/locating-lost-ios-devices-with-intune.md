---
title: Finne tapte iOS-enheter med Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440435"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Finne tapte iOS-enheter med Intune

Aktivering av tapt modus på en iOS-enhet gjør det mulig for en administrator å få en melding og kontakttelefonnummer vist på låseskjermen.

Når tapt modus er aktivert, kan administratoren bruke handlingen Finn enhet til å identifisere enhetens fysiske plassering.

Handlingen Finn enhet i Intune fungerer med iOS-enheter for å vise plasseringen av en bestemt enhet på et kart.

Bruk av denne handlingen krever at iOS-enheten er i:

- Overvåket modus
- Tapt modus

Hvis du vil ha mer informasjon, kan du se [Aktivere tapt modus på iOS/iPadOS-enheter med Intune](https://docs.microsoft.com/intune/device-lost-mode) og Finn tapte eller [stjålne iOS/iPadOS-enheter med Intune](https://docs.microsoft.com/intune/device-locate).

**SPØRSMÅL OG SVAR**

Spørsmål: Jeg utstedte en ekstern handling for å fjerne firmadata fra en enhet, og nå sitter det fast i en ventende tilstand.

Svar: For at en ekstern handling skal kunne fullføres, må den målrettede enheten være tilkoblet og sunn. I følgende situasjoner forblir den eksterne handlingen i ventende tilstand i 30 dager, eller til enheten erkjenner kommandoen:

- Når enheten ikke har tilkobling
- Når enheten mister administrasjonsstatusen med Intune

Hvis du tror at en enhet ikke lenger sjekker inn, og at den ikke kan fjerne firmadata, velger du Slett. Hvis du sletter enhetens post slik at den ikke lenger vises i Intune-listen over enheter. Hvis enheten blir aktiv igjen, må brukeren registrere den på nytt.

Spørsmål: Hvorfor er visse eksterne handlinger ikke tilgjengelige for meg å bruke?

Svar: Ikke alle plattformer støtter alle handlinger for eksterne enheter. Følgende eksterne handlinger er plattformspesifikke, så de er bare tilgjengelige for plattformene som er nevnt.

- Bypass aktiveringslås (bare iOS)
- Frisk start (bare Windows)
- Tapt modus (bare iOS)
- Finn enhet (bare iOS)
- Start på nytt (bare Windows)

Hvis du vil ha mer informasjon om hver handling, kan du se [Tilgjengelige enhetshandlinger](https://docs.microsoft.com/intune/device-management#available-device-actions).