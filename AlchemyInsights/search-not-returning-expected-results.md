---
title: 1491-søk-ikke-returnerende forventede-resultater
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709236"
---
# <a name="content-search-not-returning-expected-results"></a>Innholdssøk returnerer ikke forventede resultater

Når du kjører innholdssøk fra Microsoft 365-sikkerhets& compliance Center, kan du få uventede søkeresultater. Vurder følgende ting som kan påvirke søkeresultatene dine:

- **Innholdsplasseringer og søkebetingelser**: Kontroller at du har valgt de riktige innholdsplasseringene og søkebetingelsene. Hvis du kjørte et stort søk (med mange steder), kan du vurdere å dele det opp i flere søk.

- **Delvis indekserte elementer:** [Delvis indekserte elementer](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) fra postbokser er inkludert i de estimerte søkeresultatene. Delvis indekserte elementer fra områder i SharePoint og OneDrive er imidlertid ikke inkludert i søkeestimatet.

- **Søkefeil:** Når du søker i et stort antall postbokser (over 100 000 postbokser), kan du få søkefeil, med feilkoder som CS008-009 og CS012-002). I dette tilfellet kan du prøve søket bare for de mislykkede innholdsplasseringene. Se [denne artikkelen](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for mer informasjon.
