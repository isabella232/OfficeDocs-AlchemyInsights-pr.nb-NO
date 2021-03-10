---
title: Bruke sikkerhets baselines for Microsoft Intune til å konfigurere Windows 10-enheter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696376"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Bruke sikkerhets baselines for Microsoft Intune til å konfigurere Windows 10-enheter

Sikkerhets baselines for Intune bidrar til å beskytte brukere og enheter. Sikkerhets baselines are Windows settings's pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams. Når du oppretter en sikkerhets baseline-profil i Intune, oppretter du en mal som består av flere enhetskonfigurasjonsprofiler.

Når du distribuerer sikkerhets baselines til grupper med brukere eller enheter, brukes innstillingene på enheter som kjører på Windows 10 eller nyere versjoner. Sikkerhets baseline for administrasjon av mobilenheter (MDM) for Microsoft aktiverer for eksempel automatisk (1) BitLocker for flyttbare stasjoner, (2) krever passordet for å låse opp en enhet, og (3) deaktiverer grunnleggende godkjenning. Når en standardverdi ikke fungerer for miljøet, kan du tilpasse den opprinnelige planen slik at den bruker innstillingene du trenger.

Sikkerhets baselines also help establish an end-to-end secure workflow in Microsoft 365. Her er noen fordeler med denne funksjonaliteten:
- En sikkerhets baseline inneholder anbefalte fremgangsmåter og anbefalinger for innstillinger som påvirker sikkerhet. Fordi Intune samarbeider med Windows-sikkerhetsteamet som oppretter referanselinjer for gruppepolicyer, er disse anbefalingene basert på en solid veiledning og omfattende opplevelse.
- Hvis du ikke har brukt Intune før, og du er usikker på hvor du skal begynne, kan sikkerhets baselines hjelpe deg med å opprette og distribuere en sikker profil raskt.
- Hvis du for øyeblikket bruker en gruppepolicy, er det mye enklere å overføre til Intune for administrasjonsformål, fordi disse sikkerhets baselines er innebygd i Intune og inkluderer de aller beste funksjonene for administrasjon.

Hvis du vil ha mer informasjon, kan du se [Windows sikkerhets referanselinjer](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) og [administrasjon av mobilenheter.](https://docs.microsoft.com/windows/client-management/mdm/)