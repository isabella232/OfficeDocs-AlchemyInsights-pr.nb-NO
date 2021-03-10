---
title: Løse problemer eksternt med å onboarde Windows 10-enheter til Microsoft Defender Advanced Threat Protection
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694851"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Løse problemer eksternt med å onboarde Windows 10-enheter til Microsoft Defender Advanced Threat Protection

Hvis du har tilgang til den eksterne datamaskinen, følger du disse trinnene:

1. Last ned [diagnoseverktøyet for Client Connectivity Analyzer.](https://go.microsoft.com/fwlink/?linkid=2143466)
2. Pakk ut og kjør MDATPAnalyzer.cmd.
3. Finn diagnoseloggen i mappen MDATPClientAnalyzerResult, som er den samme mappen der verktøyet Analyzer ble lastet ned.
4. Se gjennom loggfilen for å finne problemer med tilkoblingen eller Proxy-innstillingene på Internett MDATPClientAnalyzer.txt.

Hvis du vil ha mer informasjon, [kan du se Problemer med påbordingsmaskiner.](https://go.microsoft.com/fwlink/?linkid=2143634)
