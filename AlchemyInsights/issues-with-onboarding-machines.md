---
title: Problemer med introduksjonsmaskiner
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141655"
---
# <a name="issues-with-onboarding-machines"></a>Problemer med introduksjonsmaskiner

Du kan ha problemer med introduksjonsmaskiner til MDATP-tjenesten. Hvis du har tilgang til sluttbrukermaskinen, gjør du følgende:

1. Last ned diagnoseverktøyet [Client Connectivity Analyzer.](https://aka.ms/mdatpanalyzer)
2. Pakk ut og kjør MDATPAnalyzer.cmd.
3. Finn diagnoseloggen i mappen MDATPClientAnalyzerResult, den samme mappen der Analyzer-verktøyet lastes ned.
4. Se gjennom loggfilen, MDATPClientAnalyzer.txt, for å finne problemer med tilkoblings- eller Internett-proxy-innstillinger.