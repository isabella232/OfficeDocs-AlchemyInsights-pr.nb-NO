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
ms.openlocfilehash: 5f2ed08e32694a6d7293abbabb1eddd3d251ceddbd9debf6ec3143bb4fed86db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054699"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a>Problemer med å innlemme maskiner i Microsoft Defender for endepunkter

Du kan ha problemer med å innlemme maskiner i MDE-tjenesten. Hvis du har tilgang til sluttbruker-maskinen, følg disse trinnene:

1. Last ned den siste forhåndsversjonen av diagnoseverktøyet [MDE Client Analyzer](https://aka.ms/betamdeanalyzer).
2. Høyreklikk **MDEClientAnalyzer.cmd** og velg “Kjør som administrator”.
3. Følg veiledningen som blir foreslått i **MDEClientAnalyzer.htm**.
4. For mer fyldige logger, se gjennom undermappen som ble opprettet med navn **MDEClientAnalyzerResult**.
5. Hvis du trenger ytterligere veiledning, kan du kontakte [kundestøtte for Microsoft Defender for endepunkt](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) og stille til rådighet filen MDEClientAnalyzerResult.zip for analyse.
