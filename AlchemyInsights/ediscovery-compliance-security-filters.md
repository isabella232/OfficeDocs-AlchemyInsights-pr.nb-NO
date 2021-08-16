---
title: Ingen resultater som returneres under innholdssøk/eksport
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
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101275"
---
# <a name="no-results-returned-during-content-searchexport"></a>Ingen resultater som returneres under innholdssøk/eksport

Hvis du har problemer med følgende eDiscovery-scenarier:

- Innholdssøk/eksport returnerer ingen data eller uventede data
- eDiscovery-søk eller -eksport mislykkes

Dette kan være på grunn av visse sikkerhetsfiltre for samsvar som ble konfigurert av en bestemt administrator, og som ikke ble formidlet til alle administratorer.

Du kan løse dette ved å kontrollere om det er noen sikkerhetsfiltre for samsvar som kan forårsake disse problemene:

1. Koble til sikkerhets- og samsvarssenteret Powershell
2. Kjør følgende kommandoleter:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Hvis du vil ha mer informasjon om sikkerhetsfiltre for samsvar, kan du se [Tillatelsesfiltrering for innholdssøk](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
