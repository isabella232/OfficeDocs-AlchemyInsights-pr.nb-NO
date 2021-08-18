---
title: Konfigurere personverninnstillinger i Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 991f323249e15abd137c3e69b400e40503ed30dec6507cc5071a0b1af7f72bb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090313"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>Konfigurere personverninnstillinger i Microsoft Edge

Hvis Microsoft Edge distribueres på ikke-Windows plattformer, sendes ikke diagnosedata og nettstedsinformasjon til Microsoft. Men hvis Microsoft Edge distribueres på Windows 10, sendes diagnosedata og nettstedsinformasjon i henhold til brukernes Windows [diagnosedatainnstillinger](https://go.microsoft.com/fwlink/?linkid=2132472).

Hvis du vil Microsoft Edge håndterer datainnsamling for organisasjonen, bruker du følgende gruppepolicyer:
- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) aktiverer rapportering av bruks- og krasjrelaterte data.
- [SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sender nettstedsinformasjon som brukes til å Microsoft-tjenester.

Hvis du vil ha mer informasjon, [kan du se Konfigurere policyinnstillinger](https://go.microsoft.com/fwlink/?linkid=2132577).
