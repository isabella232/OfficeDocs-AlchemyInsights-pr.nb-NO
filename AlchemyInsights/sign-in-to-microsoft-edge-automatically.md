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
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398738"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Logg på Microsoft Edge automatisk

Microsoft Edge bruker standardkontoen for operativsystemet til å logge på en bruker automatisk i henhold til hvordan brukerens enhet er konfigurert. 

Scenariene for hver type enhetskonfigurasjon og den avhengige bruker påloggingsprosessen er beskrevet nedenfor:

- **Enheten er hybrid/AAD-J**: Dette alternativet er tilgjengelig på Windows 10, windows på lavere nivå og tilsvarende serverversjoner. Brukere blir automatisk logget på med Azure Active Directory-kontoene (AD)..
- **Enheten er domeneføyd:** Dette alternativet er tilgjengelig i Windows 10, windows på lavere nivå og tilsvarende serverversjoner. Brukere med domenekontoer er som standard ikke logget på automatisk. Hvis du vil aktivere automatisk pålogging for dem, bruker du **policyen ConfigureOnPremisesAccountAutoSignIn.** Hvis du vil aktivere automatisk pålogging for brukere med Azure AD-kontoer, kan du vurdere hybridkobling av enhetene sine.
- **Operativsystemets standardkonto** er en Microsoft-konto: Dette alternativet er tilgjengelig på Windows 10 RS3 (versjon 1709, bygg 10.0.16299) og nyere versjoner. Det er usannsynlig at dette skjer på bedriftsenheter. Hvis standardkontoen for operativsystemet er en Microsoft-konto, logger Microsoft Edge imidlertid automatisk på brukeren med Microsoft-kontoen.
 
 
