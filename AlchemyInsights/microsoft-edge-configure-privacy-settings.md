---
title: Microsoft Edge konfigurere personverninnstillinger
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114181"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge konfigurere personverninnstillinger

Hvis Microsoft Edge distribueres på ikke-Windows plattformer, sendes ikke diagnosedata og nettstedsinformasjon til Microsoft. Men hvis Microsoft Edge distribueres på Windows 10, sendes diagnosedata og nettstedsinformasjon i henhold til brukernes Windows [diagnosedatainnstillinger](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).

Hvis du vil Microsoft Edge håndterer datainnsamling for organisasjonen, bruker du følgende gruppepolicyer:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Denne policyen aktiverer rapportering av bruks- og krasjrelaterte data.
- [SendSiteInfoToImproveServices:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices)Denne policyen sender nettstedsinformasjon som brukes til å Microsoft-tjenester.

Hvis du vil ha mer informasjon, [kan du se Konfigurere policyinnstillinger](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).