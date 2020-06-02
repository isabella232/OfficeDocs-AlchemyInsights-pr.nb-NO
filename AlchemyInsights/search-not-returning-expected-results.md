---
title: 1491-søk-ikke-returnerende-forventede resultater
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
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510581"
---
# <a name="content-search-not-returning-expected-results"></a>Innholdssøk returnerer ikke forventede resultater

Når du kjører innholdssøk fra Sikkerhets- & Samsvarssenter for Microsoft 365, kan du få uventede søkeresultater. Vurder følgende ting som kan påvirke søkeresultatene dine:

- **Innholdsplasseringer og søkebetingelser**: Kontroller at du har valgt de riktige innholdsplasseringene og søkevilkårene. Hvis du kjørte et stort søk (med mange steder), bør du vurdere å dele det opp i flere søk.

- **Delvis indekserte elementer**: [Delvis indekserte elementer](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) fra postbokser er inkludert i de estimerte søkeresultatene. Delvis indekserte elementer fra områder i SharePoint og OneDrive er imidlertid ikke inkludert i søkeestimatet.

- **Søksfeil**: Når du søker i et stort antall postbokser (over 100 000 postbokser), kan du få søkefeil, med feilkoder som CS008-009 og CS012-002). I dette tilfellet prøver du søket bare etter de mislykkede innholdsplasseringene. Se [denne artikkelen](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for mer informasjon.
