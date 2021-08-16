---
title: Bruk Microsoft Intune sikkerhetsgrunnlinjer til å konfigurere Windows 10 enheter
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 0a89b121f2f425b0a81fa250650f108e9af48c9da39dfc8a62b07541d3a6c3dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098071"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Bruk Microsoft Intune sikkerhetsgrunnlinjer til å konfigurere Windows 10 enheter

Intune sikkerhetsgrunnlinjer bidrar til å beskytte brukere og enheter. Sikkerhetsgrunnlinjer er Windows forhåndskonfigurerte grupper som brukes til å bruke en kjent gruppe med innstillinger og standardverdier som anbefales av de relevante sikkerhetsteamene. Når du oppretter en profil for sikkerhetsgrunnlinje i Intune, oppretter du en mal som består av flere profiler for enhetskonfigurasjon.

Når du distribuerer sikkerhetsgrunnlinjer til grupper av brukere eller enheter, brukes innstillingene på enheter som kjører på Windows 10 eller nyere. Sikkerhetsgrunnlinjen for Microsoft Mobile Device Management (MDM) aktiverer for eksempel automatisk BitLocker for flyttbare stasjoner, krever passordet for å låse opp en enhet og deaktiverer grunnleggende godkjenning. Når en standardverdi ikke fungerer for miljøet, kan du tilpasse den opprinnelige planen for å bruke innstillingene du trenger.

Sikkerhetsgrunnlinjer bidrar også til å etablere en ende-til-ende sikker arbeidsflyt i Microsoft 365. En sikkerhetsgrunnlinje inneholder anbefalte fremgangsmåter og anbefalinger for innstillinger som påvirker sikkerheten. Intune samarbeider med Windows sikkerhetsteamet som oppretter opprinnelige planer for gruppepolicyer, så disse anbefalingene er basert på solid veiledning og omfattende erfaring.

Hvis du ikke har brukt Intune før og usikker på hvor du skal begynne, kan sikkerhetsgrunnlinjer hjelpe deg med å opprette og distribuere en sikker profil raskt. Hvis du for øyeblikket bruker en gruppepolicy, er det mye enklere å overføre til Intune for administrasjonsformål med sikkerhetsgrunnlinjer fordi de er innebygd i Intune og inkluderer avanserte administrasjonsfunksjoner.

Hvis du vil ha mer [informasjon, kan du Windows sikkerhetsgrunnlinjer](/windows/security/threat-protection/windows-security-baselines) og [Administrasjon av mobilenheter](/windows/client-management/mdm/).

