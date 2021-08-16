---
title: Løse problemer med å Windows 10 enheter til Microsoft Defender Advanced Threat Protection eksternt
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
ms.openlocfilehash: 44969436c99b182cb4202fa60e2deb7d6ea3f460e48ee4649de1cfb646970f34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034043"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Løse problemer med å Windows 10 enheter til Microsoft Defender Advanced Threat Protection eksternt

Hvis du har tilgang til den eksterne datamaskinen, følger du disse trinnene:

1. Last ned [diagnoseverktøyet for Klienttilkoblingsanalyse.](https://go.microsoft.com/fwlink/?linkid=2143466)
2. Pakk ut og kjør MDATPAnalyzer.cmd.
3. Finn diagnoseloggen i MDATPClientAnalyzerResult-mappen, som er den samme mappen der analyseverktøyet ble lastet ned.
4. Hvis du vil finne problemer med tilkoblings- eller Internett-proxy-innstillinger, kan du se gjennom loggfilen MDATPClientAnalyzer.txt.

Hvis du vil ha mer informasjon, [kan du se Problemer med introduksjonsmaskiner](https://go.microsoft.com/fwlink/?linkid=2143634).
