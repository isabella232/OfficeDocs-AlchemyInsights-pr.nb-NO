---
title: Ingen resultater ble returnert under innholds søk/eksport
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727232"
---
# <a name="no-results-returned-during-content-searchexport"></a>Ingen resultater ble returnert under innholds søk/eksport

Hvis du har problemer med følgende eDiscovery-scenarioer:

- Innholds søk/eksport returnerer ingen data eller uventede data
- eDiscovery-søk eller eksport mislyktes

Dette kan skyldes bestemte sikkerhets filtre for samsvar som ble konfigurert av en bestemt administrator, og som ikke er formidlet til alle administratorer.

Du kan løse dette ved å kontrollere om det finnes noen Samsvars sikkerhets filtre som for år saker disse problemene:

1. Koble til sikkerhets-og Samsvars senteret PowerShell
2. Kjør følgende cmdleter:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Hvis du vil ha mer informasjon om Samsvars sikkerhets filtre, kan du se [tillatelses filtrering for innholds søk](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
