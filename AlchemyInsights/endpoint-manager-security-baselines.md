---
title: EndPoint Manager – sikkerhetsgrunnlinjer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421085"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager – sikkerhetsgrunnlinjer

Sikkerhetsgrunnlinjer er forhåndskonfigurerte grupper med Windows-innstillinger som hjelper deg med å bruke sikkerhetsinnstillingene som anbefales av de relevante sikkerhetsteamene. Disse grunnlinjene kan tilpasses slik at de bare leverer de ønskede innstillingene og verdiene. Hvis du vil ha mer informasjon om sikkerhetsgrunnlinjer, kan du se Bruke [sikkerhetsgrunnlinjer til å konfigurere Windows 10-enheter i Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Det finnes for øyeblikket opprinnelige planer for disse produktene:

- Sikkerhetsinnstillinger for Windows MDM
- Microsoft Defender for EndPoint Security
- Microsoft Edge

Hver av grunnlinjene oppdateres med jevne mellomrom og utgis i trinnvise versjoner. Hver versjon legger til og eller fjerner innstillinger fra den forrige versjonen for å sikre at grunnlinjen oppfyller gjeldende veiledning. Konsollen For sikkerhetsgrunnlinjer i Endepunktsikkerhet kan ulike versjoner sammenlignes ved å gjøre endringene fra versjon til versjon synlige.

Hvis du vil ha veiledning om hvordan du mest effektivt endrer hvilken versjon av opprinnelig plan som distribueres, kan du se [Behandle sikkerhetsprofiler for grunnlinje i Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Når du har distribuert en sikkerhetsgrunnlinje, kan du overvåke tilstanden til distribusjon og se gjennom innstillingene på enhet-for-enhet-basis.

**Obs!** Rapporteringsdataene for opprinnelige planer kan ta opptil 24 timer fra den første distribusjonen til en enhet og opptil seks timer for ytterligere oppdateringer. 

Den vanligste årsaken til at en innstilling for grunnlinje ikke brukes, er at den samme innstillingen brukes i en annen profil. Dette scenarioet kan undersøkes for en bestemt enhet ved å velge denne enheten fra noden Enhetsstatus for sikkerhetsgrunnlinjeprofilen. Hvis du vil ha mer informasjon, kan du se Løse [konflikter for sikkerhetsgrunnlinjer](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).