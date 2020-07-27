---
title: Retningslinjer for programbeskyttelse
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423966"
---
# <a name="application-protection-policy"></a>Retningslinjer for programbeskyttelse

Hvis du ikke har vært i bruksområdepolicy (APP) før), kan du se [oversikten over retningslinjene for appbeskyttelse](https://docs.microsoft.com/intune/apps/app-protection-policy).

Hvis du vil begynne å bruke APP, kan du se [Opprette og tilordne retningslinjer for appbeskyttelse](https://docs.microsoft.com/intune/app-protection-policies).

Krav til retningslinjer for brukspolicy:

- Brukeren har en Intune- eller EMS-lisens.
- Brukeren tilhører en gruppe som er målrettet av policyer for programbeskyttelse.
- Bare én bedriftsbruker er logget på beskyttede apper på en enhet.
- Programmet har implementert [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started). Hvis du vil ha en liste over apper som støtter SDK, kan du se [Microsoft Intune-beskyttede apper](https://docs.microsoft.com/intune/apps-supported-intune-apps).

Policyer gjelder etter at en bruker som oppfyller kravene ovenfor, logger inn i en Intune SDK-aktivert app. Den enkleste måten å finne ut om en policy brukes, er ved å kreve at brukeren angir en pin i policyen. 

Hvis du vil ha mer informasjon, kan du ta en titt på:

[Vanlige spørsmål om feilsøking av APP/MAM](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[Slik validerer du oppsettet for appbeskyttelsespolicyen](https://docs.microsoft.com/intune/app-protection-policies-validate)

[Forstå leveringstidstidspunktet for appbeskyttelsespolicy](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[Slik overvåker du retningslinjer for appbeskyttelse](https://docs.microsoft.com/intune/app-protection-policies-monitor)