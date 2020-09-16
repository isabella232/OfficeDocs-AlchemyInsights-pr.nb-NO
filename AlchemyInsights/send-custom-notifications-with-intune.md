---
title: Send egen definerte varsler med Intune
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
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720655"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Slik sender du egen definerte varsler til brukere av administrerte iOS-og Android-enheter

Egen definerte varsler for Intune behandles av Firmaportal-appen på en brukers enhet. Appen oppretter deretter push-varslingen på enheten.

Følgende er enhets krav for å støtte mottak av egen definerte varsler, og for appen oppretter du push-varslingen:

- Enheten må ha Firmaportal-appen installert.  

- Enheten må tillate at Firmaportal-appen kan sende push-varslinger. Når appen er installert eller oppdatert, blir brukeren bedt om å tillate varslinger.

- Android-enheter må ha Google Play Services installert.

- Enheten må være registrert hos Intune.

Hvis du vil ha mer informasjon, inkludert hvordan du sender en melding, kan du se [funksjons dokumentasjonen](https://docs.microsoft.com/intune/custom-notifications).
