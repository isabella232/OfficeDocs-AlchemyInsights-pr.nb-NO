---
title: Problemer med automatisk synkronisering av enhets registrering i Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714829"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Problemer med automatisk synkronisering av enhets registrering i Apple

«Vi har oppdaget at du har ett eller flere ADE-eller DEP-tokener som er i en feil tilstand. Hvis feil tilstanden er løst for hvert berørte token, vil ikke ADE-funksjonaliteten fungere for samme ".

Denne feilen kan være analyser på en rekke måter, inkludert:

1. Enheter kan ikke synkroniseres fra ABM/ASM til Intune
2. Registrerings profil tilordninger kan mislykkes
3. Det kan hende at enheter ikke full fører at ADE-registreringen ble fullført

Se etter synkroniserings feilen som ble rapportert i Intune-konsollen under **enheter > registrere enheter > Apples registrering > registrerings program-tokener** og se gjennom følgende dokumentasjon for å se mulige Utbedring:

[ABM/ASM Sync-feil for iOS/iPadOS og macOS automatiserte tokener for enhets registrering](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
