---
title: Synkroniseringsfeil ved automatisk registrering av Apple-enhet
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448931"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Synkroniseringsfeil ved automatisk registrering av Apple-enhet

«Vi har oppdaget at du har ett eller flere ADE-/DEP-tokener som er i en feiltilstand. Før feiltilstanden er løst for hvert berørte token, vil ikke ADE-funksjonaliteten fungere som forventet.

Denne feilen kan manifesteres på en rekke måter, blant annet:

1. Enheter kan ikke synkronisere fra ABM/ASM til Intune
2. Registreringsprofiltilordninger kan mislykkes
3. Det kan hende at ADE-registreringen av enheter ikke fullføres

Se etter synkroniseringsfeilen som ble rapportert i Intune-konsollen under >-enheter > **Apple-registreringstokener > registreringsprogram.**

En av de vanligste årsakene til synkroniseringsfeil er utløp av gjeldende token. I mange tilfeller vil fornyelse av det berørte tokenet løse problemet.

Hvis ett eller flere av tokenene er utløpt, kan du se følgende dokumentasjon for å hjelpe deg med å fornye dem etter behov:

[Fornye et token for automatisert enhetsregistrering](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

I tillegg kan du se følgende dokumentasjon for å se potensielle utbedringer for andre feil som forårsaker mislykkede tokensynkroniseringer:

[ABM-/ASM-synkroniseringsfeil for iOS/iPadOS og macOS-tokener for automatisert enhetsregistrering](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ABM-/ASM-synkroniseringsfeil for iOS/iPadOS og macOS-tokener for automatisert enhetsregistrering](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
