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
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919432"
---
# <a name="using-email-profiles-with-intune"></a>Bruke e-postprofiler med Intune

Intune kan brukes til å opprette og distribuere e-postprofiler for den opprinnelige (innebygde) e-postklienten på flere enhetsplattformer.

Hvis du vil ha informasjon om noen av begrensningene knyttet til e-postprofiler, inkludert hvordan tilstedeværelsen av eksisterende profiler håndteres og hvordan du fjerner e-postprofiler, kan du se Legge til e-postinnstillinger på enheter ved hjelp av [Intune](https://docs.microsoft.com/intune/email-settings-configure).

Hvis du vil ha mer informasjon om hvordan du oppretter e-postprofiler for hver enhetsplattform, kan du se:

[Innstillinger for Android-enheter for å konfigurere e-post, godkjenning og synkronisering i Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Legge til e-postinnstillinger for iOS- og iPadOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Innstillinger for e-postprofil i Microsoft Intune for enheter som Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Innstillinger for e-postprofil for enheter som Windows 10 i Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Vanlige synkroniseringsproblemer**

**En KNOX-profil på Android-e-post hindrer at brukerkontakter, kalender og oppgaver synkroniseres til brukerenheter.**

E-postprofilen KNOX på Android KNOX gir administratoren muligheten til å bestemme hvilke innholdstyper som skal synkroniseres til enheten, ved å angi at hver av dem skal aktiveres.

Hvis innstillingen for noen av innholdstypene  er satt til Ikke konfigurert (standard), synkroniseres ikke denne innholdstypen automatisk. En bruker kan aktivere innholdstypen de ønsker direkte på enheten manuelt, men denne konfigurasjonen overskrives av intune-policyinnstillingen, og synkroniseringen stopper for denne innholdstypen.

