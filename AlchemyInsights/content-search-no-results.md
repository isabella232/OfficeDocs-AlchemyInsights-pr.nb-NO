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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516788"
---
# <a name="no-results-from-content-searchexports"></a>Ingen resultater fra innhold Søk/Eksporter

Problemer med innhold Søk/eksporterer ikke returnerte noen data kan være på grunn av visse overholdelse sikkerhetsfilter som var installasjonen av et bestemt Admin og kommuniserer ikke til alle administratorer.

Hvis du vil løse dette problemet, kontrollerer du om det er samsvar sikkerhetsfiltre som kan forårsake dette:
1. Koble til sikkerhet og overholdelse Center Powershell
2. Kjør følgende kommandleter:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-$org for organisasjon