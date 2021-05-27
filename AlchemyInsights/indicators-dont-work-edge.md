---
title: Indikatorer fungerer ikke ved hjelp av Edge-nettleseren
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676461"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Indikatorer fungerer ikke ved hjelp av Edge-nettleseren

Når du har opprettet en indikator, innfris den ikke av Edge (Smartscreen). Hvis du vil ha mer informasjon, kan du se Opprette [indikatorer for NETTADRESSER og nettadresser/domener.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>Trinn 1: Sikre følgende

- Kontroller at indikatoren er riktig (ingen skrivefeil i IP/URL, riktig handling, de riktige RBAC-gruppene).
- Vent minst 2 timer etter at du har opprettet indikatoren for å ta hensyn til eventuell ventetid.
- Bekreft at systemet(e) er installert på Microsoft Defender for endepunkt.
- Kontroller at systemet(e) kan kommunisere med skyen.
- Kontroller at Smartscreen er aktivert og tilgjengelig ved å gå til [testnettstedet](https://demo.smartscreen.msft.net).

## <a name="step-2-troubleshoot-the-potential-issue"></a>Trinn 2: Feilsøke det potensielle problemet

- Kontroller at klienten oppfyller kravene. Hvis du vil ha mer informasjon, kan du se Opprette [indikatorer for NETTADRESSER og nettadresser/domener](/microsoft-365/security/defender-endpoint/indicator-ip-domain).
- Kontroller at du kjører den nyeste versjonen av Edge-nettleseren. Hvis du vil finne ut den nyeste versjonen, kan du se Finne ut hvilken [versjon av Microsoft Edge du har](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).
- Start Edge-nettleseren på nytt.
- Gå til nettstedet der du har satt opp en indikator. Hvis nettstedet ikke vises som forventet, fortsetter du til trinn 3. 

## <a name="step-3-collect-data"></a>Trinn 3: Samle inn data

- Samle **inn MDEClientAnalyzer-diagnosedata.** Hvis du vil ha instruksjoner, kan du se Problemer [med introduksjonsmaskiner til Microsoft Defender for endepunkt](issues-with-onboarding-machines.md).
- Hvis du er komfortabel med å installere og samle en Fiddler-sporing, kan du se [Telerik Fiddler](http://www.telerik.com/fiddler).
- Hvis du foretrekker veiledning fra Microsoft Kundestøtte, velger du Støtte-ikonet nedenfor for å åpne en støttesak.
