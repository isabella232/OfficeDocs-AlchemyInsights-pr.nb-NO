---
title: Intune Wi-Fi-profiler
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555315"
---
# <a name="intune-wi-fi-profiles"></a>Intune Wi-Fi-profiler

Vellykket implementering av Wi-Fi-tilkobling for MDM-klienter avhenger av en riktig distribuert profil som gjenspeiler kravene til bedriftens Wi-Fi-infrastruktur. Hvis du vil se gjennom de riktige innstillingene for klientplattformene du undersøker, kan du se: 

[Legge til Wi-Fi-innstillinger for enheter som kjører Android i Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Legge til Wi-Fi-innstillinger for Android Enterprise dedikerte og fullstendig administrerte enheter i Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Legge til Wi-Fi-innstillinger for iOS- og iPadOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Legge til Wi-Fi-innstillinger for Windows 10 og senere enheter i Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Importere Wi-Fi-innstillinger for Windows-enheter i Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Vanlige problemer**

**Jeg distribuerer en Wi-Fi-profil som er avhengig av et distribuert sertifikat som er angitt i Wi-Fi-profilen. Konfigurasjonsprofilene viser imidlertid en feilstatus.**

Kontroller at enheten mottok sertifikatet.

1. Gå til **Alle enheter i** Intune, og velg enheten > **Enhetskonfigurasjon**.

2. Kontroller at alle forventede profiler er oppført og i en vellykket tilstand.

3. For en Android-profil, hvis du har mellomliggende sertifikater i sertifikatkjeden, må du kontrollere at de distribueres til Android-enheter.

    Hvis du vil kontrollere sertifikatstatusen, går du til **Enhetskonfigurasjonsprofiler**  >  **Profiles**  >  **Android mellomliggende CA**  >  **Properties**  >  **Trusted Certificate**.

Hvis du fortsatt ser feil, kan du se gjennom avsnittene for prosedyrer og feilsøking. Hvis du vil ha mer informasjon, kan du se [Oversikt for feilsøking av SCEP-sertifikatprofiler med Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Jeg distribuerte en Wi-Fi-profil til en enhet. Intune viser at det var vellykket, men enheten kobler ikke til Wi-Fi.**

En vellykket status betyr at Intune har distribuert profilen som konfigurert. Disse konfigurasjonene samsvarer imidlertid kanskje ikke med kravene til nettverket og/eller godkjenningen. Hvis du vil ha mer informasjon om den forsøkte tilkoblingen, kan du se gjennom logger i infrastruktur- og godkjenningstjenesten (på Wi-Fi Access Point controller og NPS/Radius-serveren). Du må kanskje samarbeide med nettverksinfrastrukturteamet, eller tredjeparts Wi-Fi-leverandøren, for å samle inn og se gjennom logger.