---
title: 1491-Search-not-returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355886"
---
# <a name="content-search-not-returning-expected-results"></a>Innhold Søk returnerer ikke forventet resultat

Når du kjører innhold søk fra Office 365-sikkerhet & Center-kompatibilitet, kan du få uventede resultater. Vurder følgende ting som kan påvirke søkeresultatene:

- **Plassering av innhold og søkebetingelser**: Kontroller at du har valgt riktig innholdsplasseringer og søkevilkårene. Hvis du kjørte en stor Søk (med mange steder), kan du vurdere å dele den opp i flere søk.

- **Delvis indekserte elementer**: [delvis indekserte elementer](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) fra postbokser inkluderes i beregnet søkeresultatene. Imidlertid er delvis indekserte elementer fra områder i SharePoint og OneDrive ikke er inkludert i estimatet søk.

- **Søk-feil**: Når du søker etter et stort antall postbokser (over 100 000 postbokser), kan du få feilmeldinger når søk, med feilkoder som CS008-009 og CS012-002). I dette tilfellet, prøv Søk bare etter de mislykkede innholdsplasseringer. Se [denne artikkelen](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for mer informasjon.
