---
title: Logg på Microsoft Edge automatisk
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
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050703"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Logg på Microsoft Edge automatisk

Microsoft Edge bruker standardkontoen for operativsystemet til å logge på en bruker automatisk i henhold til hvordan brukerens enhet er konfigurert. 

Scenariene for hver type enhetskonfigurasjon og den avhengige bruker påloggingsprosessen er beskrevet nedenfor:

- **Enheten er hybrid/AAD-J**: Dette alternativet er tilgjengelig på Windows 10, Windows og tilsvarende serverversjoner. Brukere blir automatisk logget på med Azure Active Directory (AD)-kontoer.
- **Enheten er domeneføyd:** Dette alternativet er tilgjengelig på Windows 10, Windows og tilsvarende serverversjoner. Brukere med domenekontoer er som standard ikke logget på automatisk. Hvis du vil aktivere automatisk pålogging for dem, bruker du **policyen ConfigureOnPremisesAccountAutoSignIn.** Hvis du vil aktivere automatisk pålogging for brukere med Azure AD-kontoer, kan du vurdere hybridkobling av enhetene sine.
- **Operativsystemets standardkonto** er en Microsoft-konto: Dette alternativet er tilgjengelig på Windows 10 RS3 (versjon 1709, bygg 10.0.16299) og nyere versjoner. Det er usannsynlig at dette skjer på bedriftsenheter. Hvis standardkontoen for operativsystemet er en Microsoft-konto, logger Microsoft Edge brukeren automatisk med Microsoft-kontoen.
 
 
