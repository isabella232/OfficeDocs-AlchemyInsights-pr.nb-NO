---
title: Synkroniseringsfeil for automatisk registrering av Apple-enhet
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
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013757"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Synkroniseringsfeil for automatisk registrering av Apple-enhet

«Vi har oppdaget at du har ett eller flere ADE-/DEP-tokener som er i en feiltilstand. Før feilstatusen er løst for hvert berørte token, fungerer ikke ADE-funksjonaliteten som forventet.

Denne feilen kan manifestere seg på en rekke måter, inkludert:

1. Enheter synkroniseres kanskje ikke fra ABM/ASM til Intune
2. Registreringsprofiltilordninger kan mislykkes
3. Enheter fullfører kanskje ikke ADE-registreringen

Se etter synkroniseringsfeilen som ble rapportert i Intune-konsollen under Enheter > Registrere enheter > Apple-registrering > **Registreringsprogramtokener**.

En av de vanligste årsakene til synkroniseringsfeil er utløp av gjeldende token. I mange tilfeller vil fornyelse av det berørte tokenet løse problemet.

Hvis ett eller flere av tokenene er utløpt, kan du se følgende dokumentasjon for å hjelpe deg med å fornye dem etter behov:

[Fornye et token for automatisk enhetsregistrering](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

I tillegg kan du se følgende dokumentasjon for å se mulige utbedringer for andre feil som forårsaker tokensynkroniseringsfeil:

[Synkroniseringsfeil for ABM/ASM for iOS/iPadOS og macOS-tokener for automatisk registrering av enheter](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Synkroniseringsfeil for ABM/ASM for iOS/iPadOS og macOS-tokener for automatisk registrering av enheter](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
