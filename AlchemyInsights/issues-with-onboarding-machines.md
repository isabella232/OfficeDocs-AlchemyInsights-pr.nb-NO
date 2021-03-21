---
title: Problemer med å innlemme maskiner i Microsoft Defender for endepunkter
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901576"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a>Problemer med å innlemme maskiner i Microsoft Defender for endepunkter

Du kan ha problemer med å innlemme maskiner i MDE-tjenesten. Hvis du har tilgang til sluttbruker-maskinen, følg disse trinnene:

1. Last ned den siste forhåndsversjonen av diagnoseverktøyet [MDE Client Analyzer](https://aka.ms/betamdeanalyzer).
2. Høyreklikk **MDEClientAnalyzer.cmd** og velg “Kjør som administrator”.
3. Følg veiledningen som blir foreslått i **MDEClientAnalyzer.htm**.
4. For mer fyldige logger, se gjennom undermappen som ble opprettet med navn **MDEClientAnalyzerResult**.
5. Hvis du trenger ytterligere veiledning, kan du kontakte [kundestøtte for Microsoft Defender for endepunkt](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) og stille til rådighet filen MDEClientAnalyzerResult.zip for analyse.
