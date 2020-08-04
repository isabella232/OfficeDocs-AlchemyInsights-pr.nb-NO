---
title: Bruke e-postprofiler med Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555250"
---
# <a name="using-email-profiles-with-intune"></a>Bruke e-postprofiler med Intune

Intune kan brukes til å opprette og distribuere e-postprofiler for den opprinnelige (innebygde) e-postklienten på flere enhetsplattformer.

Hvis du vil ha informasjon om noen av begrensningene som er knyttet til e-postprofiler, inkludert hvordan tilstedeværelsen av eksisterende profiler håndteres og hvordan du fjerner e-postprofiler, kan du se Legge til [e-postinnstillinger på enheter ved hjelp av Intune](https://docs.microsoft.com/intune/email-settings-configure).

Hvis du vil ha mer informasjon om hvordan du oppretter e-postprofiler for hver enhetsplattform, kan du se:

[Innstillinger for Android-enheter for å konfigurere e-post, godkjenning og synkronisering i Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Legge til e-postinnstillinger for iOS- og iPadOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Innstillinger for e-postprofil i Microsoft Intune for enheter som kjører Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Innstillinger for e-postprofil for enheter som kjører Windows 10 i Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Vanlige synkroniseringsproblem**

**En KNOX på Android-e-postprofil hindrer at brukerkontakter, kalender og oppgaver synkroniseres til brukerenheter.**

KNOX på Android KNOX-e-postprofilen gir administratoren muligheten til å bestemme hvilke innholdstyper som synkroniseres med enheten ved å angi at hver av dem er aktivert.

Hvis innstillingen for noen av innholdstypene er satt til **Ikke konfigurert** (standard), synkroniseres ikke denne innholdstypen automatisk. En bruker kan aktivere innholdstypen de vil ha direkte på enheten manuelt, men denne konfigurasjonen overskrives av policyinnstillingen Intune, og synkroniseringen stopper for denne innholdstypen.

