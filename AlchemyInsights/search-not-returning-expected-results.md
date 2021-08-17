---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052719"
---
# <a name="content-search-not-returning-expected-results"></a>Innholdssøk returnerer ikke forventede resultater

Når du kjører innholdssøk fra Microsoft 365 sikkerhets- & samsvarssenteret, kan du få uventede søkeresultater. Vurder følgende ting som kan påvirke søkeresultatene:

- **Innholdsplasseringer og søkebetingelser**: Kontroller at du har valgt riktige innholdsplasseringer og søkebetingelser. Hvis du kjørte et stort søk (med mange plasseringer), bør du vurdere å dele det inn i flere søk.

- **Delvis indekserte elementer**:  [Delvis indekserte elementer](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) fra postbokser er inkludert i de beregnede søkeresultatene. Delvis indekserte elementer fra områder i SharePoint og OneDrive er imidlertid ikke inkludert i søkeestimatet.

- **Søkefeil:** Når du søker i et stort antall postbokser (over 100 000 postbokser), kan du få søkefeil, med feilkoder som CS008-009 og CS012-002). I dette tilfellet kan du bare søke på nytt etter plasseringer med mislykkede innhold. Se  [denne artikkelen](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) hvis du vil ha mer informasjon.
