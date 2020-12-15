---
title: Microsoft Edge konfigurere person vern innstillinger
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
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677797"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge konfigurere person vern innstillinger

Hvis Microsoft Edge distribueres på ikke-Windows-plattformer som standard, sendes ikke diagnose data og område informasjon til Microsoft. Hvis imidlertid Microsoft Edge distribueres på Windows 10, sendes diagnose data og område informasjon i henhold til brukernes [Windows diagnose data innstillinger](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).

Hvis du vil konfigurere hvordan Microsoft Edge behandler data innsamling for organisasjonen, bruker du følgende gruppe policyer:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): denne policyen muliggjør rapportering av bruk og krasj relaterte data.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): denne policyen sender nettsteds informasjon som brukes til å forbedre Microsoft-tjenester.

Hvis du vil ha mer informasjon, kan du se [konfigurere policy innstillinger](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).