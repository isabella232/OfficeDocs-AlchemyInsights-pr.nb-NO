---
title: Innholds søk ingen resultater
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680656"
---
# <a name="no-results-from-content-searchexports"></a>Ingen resultater fra innholds søk/eksporterer

Problemer med innholds søk/Eksporter som ikke returnerer data, kan være på grunn av bestemte sikkerhets filtre for samsvar som ble konfigurert av en bestemt administrator, og ikke formidle det til alle administratorer.

Du kan løse dette ved å kontrollere om det finnes noen Samsvars sikkerhets filtre som gjør dette:
1. Koble til sikkerhets-og Samsvars senteret PowerShell
2. Kjør følgende cmdleter:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-Organization $org