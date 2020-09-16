---
title: 1491 – søk – ikke returnert – forventet resultat
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
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740483"
---
# <a name="content-search-not-returning-expected-results"></a>Innholds søk returnerer ikke forventede resultater

Når du kjører innholds søk fra sikkerhets & Samsvars senteret i Microsoft 365, kan det hende du får uventede søke resultater. Vurder følgende ting som kan påvirke søke resultatene:

- **Innholds plasseringer og søke betingelser**: Kontroller at du har valgt riktige innholds plasseringer og søke vilkårene. Hvis du kjørte et stort søk (med mange plasseringer), bør du vurdere å dele det inn i flere søk.

- **Delvis indekserte elementer**:  [delvis indekserte elementer](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) fra post bokser er inkludert i de beregnede søke resultatene. Delvis indekserte elementer fra nett steder i SharePoint og OneDrive er imidlertid ikke inkludert i søke estimatet.

- **Søke feil**: Når du søker etter et stort antall post bokser (over 100 000 post bokser), kan du få søke feil, med feil koder som CS008-009 og CS012-002). I dette tilfellet må du prøve søket på nytt bare for de mislykkede innholds plasseringene. Se  [denne artikkelen](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) hvis du vil ha mer informasjon.
