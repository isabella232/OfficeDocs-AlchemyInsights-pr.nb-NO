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
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405102"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>Konfigurere personverninnstillinger i Microsoft Edge

Hvis Microsoft Edge distribueres på ikke-Windows-plattformer, sendes som standard ikke diagnosedata og nettstedsinformasjon til Microsoft. Hvis Microsoft Edge er distribuert på Windows 10, sendes imidlertid diagnosedata og nettstedsinformasjon i henhold til brukernes [datainnstillinger for Windows Diagnostic](https://go.microsoft.com/fwlink/?linkid=2132472).

Hvis du vil konfigurere hvordan Microsoft Edge håndterer datainnsamling for organisasjonen, bruker du følgende gruppepolicyer:
- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) aktiverer rapportering av bruks- og krasjrelaterte data.
- [SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sender nettstedsinformasjon som brukes til å forbedre Microsoft-tjenester.

Hvis du vil ha mer informasjon, [kan du se Konfigurere policyinnstillinger](https://go.microsoft.com/fwlink/?linkid=2132577).
