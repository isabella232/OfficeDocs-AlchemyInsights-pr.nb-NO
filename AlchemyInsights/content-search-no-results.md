---
title: Innholdssøk uten resultater
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816857"
---
# <a name="no-results-from-content-searchexports"></a>Ingen resultater fra Innholdssøk/eksporter

Problemer med innholdssøk/eksporter som ikke returnerer data, kan være på grunn av visse sikkerhetsfilter for samsvar som ble satt opp av en bestemt administrator og ikke kommuniserer det til alle administratorer.

Du kan løse dette ved å kontrollere om det finnes samsvarssikkerhetsfiltre som kan forårsake dette:
1. Koble til Powershell for sikkerhets- og samsvarssenteret
2. Kjør følgende kommandoleter:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org