---
title: Sende egendefinerte varslinger med Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992321"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Slik sender du tilpassede varslinger til brukere av administrerte iOS-og Android-enheter

Tilpassede varslinger for Intune behandles av Company Portal-appen på en brukers enhet. Appen oppretter deretter push-varslingen på den enheten.

Følgende er enhets forutsetninger for å støtte mottak av egendefinerte varslinger, og for appen å deretter opprette push-varsling:

- Enheten må ha Company Portal-appen installert.  

- Enheten må tillate at Company Portal-appen sender push-varslinger. Når appen er installert eller oppdatert, vil den be brukeren om å tillate varslinger.

- Android-enheter må ha Google Play Services installert.

- Enheten må være registrert i Intune.

Hvis du vil ha mer informasjon, inkludert hvordan du sender en melding, kan du se [funksjons dokumentasjonen](https://docs.microsoft.com/intune/custom-notifications).
