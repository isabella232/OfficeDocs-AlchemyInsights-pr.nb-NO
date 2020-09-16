---
title: Bruke e-postprofiler med Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653297"
---
# <a name="using-email-profiles-with-intune"></a>Bruke e-postprofiler med Intune

Intune kan brukes til å opprette og distribuere e-postprofiler for den opprinnelige (innebygde) e-postklienten på flere enhets plattformer.

Hvis du vil ha informasjon om noen av begrensningene som er knyttet til e-postprofiler, inkludert hvordan eksisterende profiler håndteres, og hvordan du fjerner e-postprofiler, kan du se [legge til e-postinnstillinger i enheter ved](https://docs.microsoft.com/intune/email-settings-configure)

Hvis du vil ha mer informasjon om hvordan du oppretter e-postprofiler for hver enhets plattform, kan du se:

[Innstillinger for Android-enhet konfigurere e-post, godkjenning og synkronisering i Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Legge til e-postinnstillinger for iOS-og iPadOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Innstillinger for e-postprofil i Microsoft Intune for enheter som kjører Windows Phone 8,1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Innstillinger for e-postprofil for enheter som kjører Windows 10 i Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Vanlig synkroniserings problem**

**En KNOX on Android-e-postprofil hindrer at bruker kontakter, kalender og oppgaver synkroniseres til bruker enheter.**

KNOX på Android KNOX-e-postprofilen gir administratorer muligheten til å bestemme hvilke innholds typer som skal synkroniseres til enheten ved å angi hver til aktivert.

Hvis innstillingen for noen av innholds typene er satt til **ikke konfigurert** (standard), synkroniseres ikke denne innholds typen automatisk. En bruker kan aktivere innholds typen de ønsker direkte på enheten manuelt, men denne konfigurasjonen overskrives av policy innstillingen Intune, og synkroniserings stoppet for denne innholds typen.

