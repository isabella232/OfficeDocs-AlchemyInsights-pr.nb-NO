---
title: Bruk Microsoft Intune sikkerhetsgrunnlinjer til å konfigurere Windows 10 enheter
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104353"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Bruk Microsoft Intune sikkerhetsgrunnlinjer til å konfigurere Windows 10 enheter

Intune sikkerhetsgrunnlinjer bidrar til å beskytte brukere og enheter. Sikkerhetsgrunnlinjer er Windows forhåndskonfigurerte grupper som brukes til å bruke en kjent gruppe med innstillinger og standardverdier som anbefales av de relevante sikkerhetsteamene. Når du oppretter en profil for sikkerhetsgrunnlinje i Intune, oppretter du en mal som består av flere profiler for enhetskonfigurasjon.

Når du distribuerer sikkerhetsgrunnlinjer til grupper av brukere eller enheter, brukes innstillingene på enheter som kjører på Windows 10 eller nyere. MDM Security Baseline aktiverer for eksempel automatisk (1) BitLocker for flyttbare stasjoner, (2) krever passordet for å låse opp en enhet, og (3) deaktiverer enkel godkjenning. Når en standardverdi ikke fungerer for miljøet, tilpasser du den opprinnelige planen for å bruke innstillingene du trenger.

Sikkerhetsgrunnlinjer bidrar også til å etablere en ende-til-ende sikker arbeidsflyt i Microsoft 365. Følgende er noen fordeler med dette:

- En sikkerhetsgrunnlinje inneholder anbefalte fremgangsmåter og anbefalinger for innstillinger som påvirker sikkerheten. Siden Intune samarbeider med Windows sikkerhetsteamet som oppretter opprinnelige planer for gruppepolicyer, er disse anbefalingene basert på solid veiledning og omfattende erfaring.
- Hvis du ikke har brukt Intune før og usikker på hvor du skal begynne, vil sikkerhetsgrunnlinjer hjelpe deg med å opprette og distribuere en sikker profil raskt.
- Hvis du for øyeblikket bruker en gruppepolicy, er det mye enklere å overføre til Intune for administrasjonsformål, fordi de er innebygd i Intune og inkluderer avanserte funksjoner for administrasjon.

Hvis du vil ha mer [informasjon, kan du Windows sikkerhetsgrunnlinjer](https://go.microsoft.com/fwlink/?linkid=2141503) og [Administrasjon av mobilenheter](https://go.microsoft.com/fwlink/?linkid=2141701).