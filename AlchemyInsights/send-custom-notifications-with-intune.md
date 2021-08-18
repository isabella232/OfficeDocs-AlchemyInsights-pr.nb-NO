---
title: Sende egendefinerte varsler med Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086173"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Slik sender du egendefinerte varsler til brukere av administrerte iOS- og Android-enheter

Egendefinerte varsler for Intune behandles av firmaportal-appen på en brukers enhet. Appen oppretter deretter push-varslingen på den enheten.

Følgende er enhetskrav for å støtte mottak av egendefinerte varsler, og for at appen skal kunne opprette push-varslingen:

- Enheten må ha firmaportal-appen installert.  

- Enheten må tillate at appen firmaportal sende push-varslinger. Når appen er installert eller oppdatert, blir brukeren bedt om å tillate varslinger.

- Android-enheter må ha Google Play-tjenester installert.

- Enheten må være registrert med Intune.

Hvis du vil ha mer informasjon, inkludert hvordan du sender en melding, kan du se [funksjonsdokumentasjonen](https://docs.microsoft.com/intune/custom-notifications).
