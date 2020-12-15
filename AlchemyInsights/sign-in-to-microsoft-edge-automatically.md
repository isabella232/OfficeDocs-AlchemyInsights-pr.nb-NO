---
title: Logge på Microsoft Edge automatisk
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677769"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Logge på Microsoft Edge automatisk

Microsoft Edge bruker operativ systemets standard konto til automatisk å logge seg på en bruker i henhold til hvordan brukerens enhet er konfigurert. 

Scenariene for hver type enhets konfigurasjon og den avhengige bruker påloggings prosessen beskrives nedenfor:

1. **Enheten er hybrid/AAD-J**: dette alternativet er tilgjengelig i Windows 10, Windows på lavere nivå og tilsvarende serverversjoner. Brukere logges automatisk på med Azure Active Directory-kontoer (AD).
2. **Enheten er domene tilknyttet**: dette alternativet er tilgjengelig i Windows 10, Windows på lavere nivå og tilsvarende serverversjoner. Som standard logges ikke brukere med domene kontoer automatisk. Hvis du vil aktivere automatisk pålogging for dem, bruker du **ConfigureOnPremisesAccountAutoSignIn** -policyen. Hvis du vil aktivere automatisk pålogging for brukere med Azure AD-kontoer, bør du vurdere å bli med i hybrid tilkobling til enhetene sine.
3. **Standard kontoen for operativ systemet er en Microsoft-konto**: dette alternativet er tilgjengelig på Windows 10 RS3 (versjon 1709, bygg 10.0.16299) og nyere versjoner. Det er lite sannsynlig at scenarioet oppstår på bedrifts enheter. Hvis for eksempel operativ systemets standard konto er en Microsoft-konto, logger Microsoft Edge automatisk på brukeren med Microsoft-kontoen.
 
 
