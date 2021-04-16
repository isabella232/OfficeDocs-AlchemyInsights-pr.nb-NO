---
title: Eksportverktøy for eDiscovery
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814597"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kan du ikke installere eller kjøre eksportverktøyet for eDiscovery?

Hvis du ikke kan installere eller kjøre eksportverktøyet for eDiscovery for å laste ned søkeresultater, kontrollerer du følgende:
  
- Datamaskinen du bruker, oppfyller disse forhåndskravene:

  - 32- eller 64-biters versjoner av Windows 7 og nyere versjoner

  - Microsoft .NET Framework 4.7

  - En støttet nettleser:

  - Microsoft Edge

    eller

  - Internet Explorer 10 og nyere versjoner

    Andre nettlesere, for eksempel Google Chrome og Mozilla Firefox, støttes ikke.

- Organisasjonen kan koble til endepunktet i Azure, som er **\* .blob.core.windows.net** (jokertegnet representerer en unik identifikator for eksportjobben).

- Du er tilordnet eksportrollen i sikkerhetssamsvarssenteret for Microsoft 365. &amp; Denne rollen tilordnes som standard bare til rollegruppen eDiscovery Manager. Se [Tilordne eDiscovery-tillatelser](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Hvis du vil ha mer informasjon, [kan du se Eksportere søkeresultater for innhold](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Hvis du eksporterer mer enn 100 000 postbokser, må du bruke følgende Powershell til å laste ned eksportresultatene: Eksportere resultater fra mer enn  [100 000 postbokser](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).