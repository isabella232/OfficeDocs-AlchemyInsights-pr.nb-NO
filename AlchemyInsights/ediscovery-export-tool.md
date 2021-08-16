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
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101311"
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

- Du er tilordnet eksportrollen i sikkerhetssamsvarssenteret Microsoft 365 &amp; sikkerhetssamsvar. Denne rollen tilordnes som standard bare til rollegruppen eDiscovery Manager. Se [Tilordne eDiscovery-tillatelser](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Hvis du vil ha mer informasjon, [kan du se Eksportere søkeresultater for innhold](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Hvis du eksporterer mer enn 100 000 postbokser, må du bruke følgende Powershell til å laste ned eksportresultatene: Eksportere resultater fra mer enn  [100 000 postbokser](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).