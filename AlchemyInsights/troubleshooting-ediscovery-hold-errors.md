---
title: Feilsøking av ediscovery inneholder feil
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676277"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Feilsøking av ediscovery inneholder feil

Har du problemer med eDiscovery-sperringer? Her er noen anbefalte fremgangsmåter du bør vurdere:

- Kontroller sperredistribusjonsstatusen.  Hvis statusen er **På (venter)** eller **Av (venter),** venter du på at sperrefordelingen skal fullføres.
- Slå sammen oppdateringer for eDiscovery-sperring til én enkelt masseforespørsel i stedet for å oppdatere policyen gjentatte ganger for hver transaksjon.
- Kjør Set-CaseHoldPolicy <policyname> -RetryDistribution i Powershell for sikkerhets- og samsvarssenteret. Hvis du vil ha mer [informasjon, kan du Koble til sikkerhets-& PowerShell](/powershell/exchange/connect-to-scc-powershell).

Hvis du vil ha fremgangsmåter for å kontrollere disse innstillingene og flere anbefalte fremgangsmåter for å begrense og løse problemer med eDiscovery-sperringer, kan du se Feilsøke [problemer med sperring av eDiscovery](/microsoft-365/compliance/hold-distribution-errors).
Hvis du vil ha informasjon om feilsøking av andre vanlige eDiscovery-problemer, kan du se Undersøke, feilsøke og løse vanlige [eDiscovery-problemer](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).
