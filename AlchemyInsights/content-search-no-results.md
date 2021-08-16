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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058011"
---
# <a name="no-results-from-content-searchexports"></a>Ingen resultater fra Innholdssøk/eksporter

Problemer med innholdssøk/eksporter som ikke returnerer data, kan være på grunn av visse sikkerhetsfilter for samsvar som ble satt opp av en bestemt administrator og ikke kommuniserer det til alle administratorer.

Du kan løse dette ved å kontrollere om det finnes samsvarssikkerhetsfiltre som kan forårsake dette:
1. Koble til sikkerhets- og samsvarssenteret Powershell
2. Kjør følgende kommandoleter:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org