---
title: Regler for reduksjon av angrepsoverflater
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
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676437"
---
# <a name="attack-surface-reduction-rules"></a>Regler for reduksjon av angrepsoverflater

Hvis du utelater filer eller mapper, kan beskyttelsen som leveres av regler for reduksjon av angrepsoverflater, reduseres kraftig. Filer som ville ha blitt blokkert av en regel, kan kjøres, og ingen rapport eller hendelse registreres. En utelatelse gjelder for alle regler som tillater utelatelser.

ASR-utelatelser bruker samme syntaks som Microsoft Defender Antivirus utelatelser. Hvis du vil ha mer informasjon, kan du se Konfigurere og validere [utelatelser for Microsoft Defender Antivirus skanninger](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus). Hvis du vil unngå problemer, kan du se gjennom Vanlige feil du [bør unngå når du definerer utelatelser.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)

Ikke alle ASR-regler støtter utelatelser. Hvis du vil validere om regelen støtter utelatelser, kan du se tabellen [Angrepsoverflatereduksjonsregler](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

## <a name="attack-surface-reduction-rules"></a>Regler for reduksjon av angrepsoverflater

Organisasjonens angrepsoverflate omfatter alle stedene der en angriper kan kompromittere organisasjonsenheter eller -nettverk. Reduksjon av angrepsoverflaten betyr å beskytte organisasjonsenhetene og nettverket, noe som gjør at angripere med færre måter å utføre angrep på. Det kan hjelpe å konfigurere regler for reduksjon av angrepsoverflater i Microsoft Defender for endepunkt.

Hvis du vil ha mer informasjon, kan du se:

- [Tilordne GUID for ASR-regel til navn](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- ASR-regler:
    - [Windows 10 Pro, versjon 1709 eller nyere](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, versjon 1709 eller nyere](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, versjon 1803 (halvårskanal) eller nyere](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Identifiser riktig utelatelse som skal brukes

1. Se etter hendelses-ID 1121 eller 1122 i Microsoft-Windows-Windows Defender/Operativ logg.

1. Evaluer blokkscenarioet og konteksten, og bekreft at dette scenarioet må oppheves.

1. Les Bane-verdien i hendelsesdetaljene, som er verdien som definerer utelatelsen.
    - Gjør utelukkelsen så streng som mulig.
    - Bruk et jokertegn der det er nødvendig (for eksempel erstatt brukervariabel).

1. Bruk utelukkelsen i henhold til distribusjonsbehovene dine. Hvis du vil ha mer informasjon, kan du [se Tilpasse regler for reduksjon av angrepsoverflater](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).

## <a name="exclusion-is-not-honored"></a>Utelukkelse er ikke innfridd

1. Bestem om regelen støtter utelatelser. Hvis du vil ha mer informasjon, [kan du se Regler for reduksjon av angrepsoverflater](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

1. Se gjennom utelatelsene som er brukt, og bekreft med hendelsesdataene for skrivefeil eller feiltoolerte jokertegn. Hvis du vil ha mer informasjon, kan du [se Utelukkelsestyper som støttes](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. Hvis regelen påvirkes for høyt, bør du vurdere å flytte regelen (tilbake) til overvåkingsmodus for å utføre ytterligere validering. Hvis du vil ha mer informasjon, kan du se [Teste hvordan Microsoft Defender for endepunktfunksjoner fungerer i overvåkingsmodus](/microsoft-365/security/defender-endpoint/audit-windows-defender).

1. Samle inn støttedata for å åpne en støttesak ved hjelp av denne kommandoen:
    
   ** MDEClientAnalyzer.cmd -v**

    Hvis du vil ha mer informasjon, kan du se [Problemer med introduksjonsmaskiner til Microsoft Defender for endepunkter](issues-with-onboarding-machines.md).
