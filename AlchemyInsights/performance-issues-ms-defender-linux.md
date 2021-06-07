---
title: Ytelsesproblemer for Microsoft Defender for endepunkt på Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794003"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Ytelsesproblemer for Microsoft Defender for endepunkt på Linux

Denne artikkelen veileder deg gjennom trinnene for å identifisere ytelsesproblemer for Microsoft Defender for endepunkt på Linux.

Det er viktig å først kontrollere at problemet du opplever, er løst med [den nyeste versjonen.](/microsoft-365/security/defender-endpoint/linux-whatsnew) 

Hvis du vil starte undersøkelsen, kan du se [Feilsøke ytelsesproblemer for Microsoft Defender for endepunkt på Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>Utelatelser

Utelatelser kan bidra til å redusere ytelsesproblemer. Se gjennom utelatelsene før du begynner, slik at eventuell ekstra risiko er kjent og dokumentert.

Hvis du vil ha mer informasjon, kan du se Konfigurere og validere utelatelser [for Microsoft Defender for endepunkt på Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).

Når du har flere filer & mapper som skal utelates, og alle er på samme monteringspunkt, kan det være enklere å utelate monteringspunktet. Fra og med februarutgivelse 101.22.80 kan du utelate et helt monteringspunkt.

Hvis for eksempel /mnt/backup er et monteringspunkt, kan du legge til /mnt/backup i ekskluderingslisten ved å kjøre denne kommandoen:

`$ mdatp exclusion folder add –path /mnt/backup`

**Obs!** Hvis du legger til utelatelser, øker risikoen for at skadelig programvare ikke oppdages og bør håndteres og implementeres med forsiktighet.

## <a name="need-help"></a>Trenger du hjelp?

Hvis du vil hjelpe deg på den mest effektive måten, kan du samle inn diagnosedataene før du åpner en støttesak.
