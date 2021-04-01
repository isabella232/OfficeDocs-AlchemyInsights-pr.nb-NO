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
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440893"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager – sikkerhetsgrunnlinjer

Sikkerhetsgrunnlinjer er forhåndskonfigurerte grupper med Windows-innstillinger som hjelper deg med å bruke sikkerhetsinnstillingene som anbefales av de relevante sikkerhetsteamene. Disse referanseverdiene kan tilpasses for bare å levere de innstillingene og verdiene du ønsker. Hvis du vil ha mer informasjon om sikkerhetsmessige grunnlinjer, kan du se [Bruk sikkerhetsmessige grunnlinjer til å konfigurere Windows 10-enheter i Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Det finnes for øyeblikket grunnlinjer for disse produktene:

- Windows MDM-sikkerhetsinnstillinger
- Microsoft Defender for EndPoint Security
- Microsoft Edge

Hver av grunnlinjene oppdateres med jevne mellomrom og lanseres i trinnvise versjoner. Hver versjon legger til og fjerner innstillinger fra den forrige versjonen for å sikre at grunnlinjen oppfyller gjeldende veiledning. Sikkerhetskonsollen for grunnlinjer i Endepunktsikkerhet tillater ulike versjoner å sammenlignes ved å gjøre endringene fra versjon til versjon synlig.

Hvis du vil ha veiledning i hvordan du mest effektivt endrer hvilken versjon av grunnlinje som distribueres, kan du se [Behandle profiler for sikkerhetsgrunnlinjer i Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Når du har distribuert en grunnkonfigurasjon for sikkerhet, kan du overvåke tilstanden til distribusjonen og se gjennom innstillingene på enhetsbasis.

**Merk:** Det kan ta opptil 24 timer før rapporteringsdataene for grunnlinjer vises fra den første distribusjonen til en enhet, og opptil seks timer for ytterligere oppdateringer. 

Den vanligste årsaken til at en grunnlinje-innstilling ikke brukes, er at den samme innstillingen brukes i en annen profil. Dette scenarioet kan undersøkes for bestemte enheter ved å velge den aktuelle enheten fra Enhetsstatus-noden i profilen for Grunnkonfigurasjon for sikkerhet. Hvis du vil ha mer informasjon, kan du se [Løse konflikter for grunnkonfigurasjoner for sikkerhet](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).