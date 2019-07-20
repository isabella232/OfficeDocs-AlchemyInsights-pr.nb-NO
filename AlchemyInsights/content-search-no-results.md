---
title: Ingen resultat av søk innhold
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800490"
---
# <a name="no-results-from-content-searchexports"></a>Ingen resultater fra innhold Søk/Eksporter

Problemer med innhold Søk/eksporterer ikke returnerte noen data kan være på grunn av visse overholdelse sikkerhetsfilter som var installasjonen av et bestemt Admin og kommuniserer ikke til alle administratorer.

Hvis du vil løse dette problemet, kontrollerer du om det er samsvar sikkerhetsfiltre som kan forårsake dette:
1. Koble til sikkerhet og overholdelse Center Powershell
2. Kjør følgende kommandleter:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-$org for organisasjon