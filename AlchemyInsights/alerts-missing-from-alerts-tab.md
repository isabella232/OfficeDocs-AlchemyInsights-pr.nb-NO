---
title: Varsler mangler i Varsler-fanen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12732"
ms.openlocfilehash: 9fbd9a32e40d858f0ba49931c723a824478aaa12
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454972"
---
# <a name="alerts-missing-from-alerts-tab"></a>Varsler mangler i Varsler-fanen

**Varsler-fanen** fungerer basert på oppsett og aktiverte policyer fra appstyringsportalen i leieren. Out-of-the-box policies in App Governance also must be activated to let signals flow to the **Alerts tab.** 

Bekreft at varselet er generert:

1. Gå til policyer for [appstyring,](https://compliance.microsoft.com/m365appprotection?viewid=policies) og bekreft at du har opprettet minst én aktiv policy eller overvåkingspolicy.

1. Velg policyen, og seleect **Rediger** i undermenyruten. 

1. Kontroller policykonfigurasjonen for å bekrefte at et varsel skal ha blitt generert basert på en policyhendelse som ble startet for mer enn 24 timer siden.

Hvis du vil ha mer informasjon om varsler i App governance, kan du se Komme i gang med [gjenkjenning](https://docs.microsoft.com/microsoft-365/compliance/app-governance-detect-remediate-get-started)og utbedring av apptrusler.