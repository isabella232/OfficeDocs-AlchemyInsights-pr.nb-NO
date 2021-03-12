---
title: Løse problemer med å installere Windows 10-enheter eksternt til Microsoft Defender Advanced Threat Protection
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750037"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Løse problemer med å installere Windows 10-enheter eksternt til Microsoft Defender Advanced Threat Protection

Hvis du har tilgang til den eksterne datamaskinen, følger du disse trinnene:

1. Last ned [diagnoseverktøyet for Klienttilkoblingsanalyse.](https://go.microsoft.com/fwlink/?linkid=2143466)
2. Pakk ut og kjør MDATPAnalyzer.cmd.
3. Finn diagnoseloggen i MDATPClientAnalyzerResult-mappen, som er den samme mappen der analyseverktøyet ble lastet ned.
4. Hvis du vil finne problemer med tilkoblings- eller Internett-proxy-innstillinger, kan du se gjennom loggfilen MDATPClientAnalyzer.txt.

Hvis du vil ha mer informasjon, [kan du se Problemer med introduksjonsmaskiner](https://go.microsoft.com/fwlink/?linkid=2143634).
