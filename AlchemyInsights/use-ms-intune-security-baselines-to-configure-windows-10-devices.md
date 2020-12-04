---
title: Bruke sikkerhets planer for Microsoft Intune til å konfigurere Windows 10-enheter
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
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573536"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Bruke sikkerhets planer for Microsoft Intune til å konfigurere Windows 10-enheter

Sikkerhets opprinnelige planer for Intune bidrar til å beskytte brukere og enheter. Sikkerhets opprinnelige planer er Windows-innstillinger, forhånds kon figurerte grupper brukes til å bruke en kjent gruppe med innstillinger og standard verdier som anbefales av de aktuelle sikkerhets teamene. Ved å opprette en opprinnelig basis profil i Intune, oppretter du en mal som består av flere profiler for enhets konfigurasjon.

Når du distribuerer sikkerhets opprinnelige planer til grupper av brukere eller enheter, gjelder innstillingene for enheter som kjører på Windows 10 eller nyere. MDM-sikkerhet for sikkerhets plan automatisk (1) aktiverer for eksempel BitLocker for flyttbare stasjoner (2) krever passordet for å låse opp en enhet, og (3) deaktiverer enkel godkjenning. Når en standard verdi ikke fungerer for miljøet ditt, kan du tilpasse den opprinnelige planen for å bruke innstillingene du trenger.

Sikkerhets opprinnelige planer bidrar også til å opprette en slutt-til-ende sikker arbeids flyt i Microsoft 365. Følgende er noen av fordelene med dette:

- En sikkerhets plan omfatter anbefalte Fremgangs måter og anbefalinger for innstillinger som påvirker sikkerheten. Siden Intune-partnere med Windows-sikkerhetsmaskinvaren som oppretter opprinnelige planer for gruppe policyer, er disse anbefalingene basert på solid veiledning og omfattende opplevelse.
- Hvis du ikke har brukt Intune og ikke vet hvor du skal begynne, kan sikkerhets opprinnelige planer gjøre det enklere å opprette og distribuere en sikker profil.
- Hvis du for øyeblikket bruker en gruppe policy, er det mye enklere å overføre til Intune for administrasjons formål, fordi de er innebygd i Intune og inkludere de kuttede funksjonene for administrasjon.

Hvis du vil ha mer informasjon, kan du se [sikkerhets opprinnelige planer for Windows](https://go.microsoft.com/fwlink/?linkid=2141503) og [administrasjon av mobil enheter](https://go.microsoft.com/fwlink/?linkid=2141701).