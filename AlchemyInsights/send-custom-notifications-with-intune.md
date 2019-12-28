---
title: Sende egendefinerte varslinger med Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886866"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Slik sender du tilpassede varslinger til brukere av administrerte iOS-og Android-enheter

Tilpassede varslinger for Intune behandles av Company Portal-appen på en brukers enhet. Appen oppretter deretter push-varslingen på den enheten.

Følgende er enhets forutsetninger for å støtte mottak av egendefinerte varslinger, og for appen å deretter opprette push-varsling:

- Enheten må ha Company Portal-appen installert.  

- Enheten må tillate at Company Portal-appen sender push-varslinger. Når appen er installert eller oppdatert, vil den be brukeren om å tillate varslinger.

- Android-enheter må ha Google Play Services installert.

- Enheten må være registrert i Intune.

Hvis du vil ha mer informasjon, inkludert hvordan du sender en melding, kan du se [funksjons dokumentasjonen](https://docs.microsoft.com/intune/custom-notifications).
