---
title: eDiscovery eksportverktøy
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 6352603a391ddcb44d2728c7587bf15a6cd97ebb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507179"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kan du ikke installere eller kjøre eDiscovery Export Tool?

Hvis du ikke kan installere eller kjøre eDiscovery Export Tool for å laste ned søkeresultater, kan du kontrollere følgende ting:
  
- Datamaskinen du bruker, oppfyller disse forutsetningene:

  - 32- eller 64-biters versjoner av Windows 7 og senere versjoner

  - Microsoft .NET Framework 4.7

  - En støttet nettleser:

  - Microsoft Edge

    eller

  - Internet Explorer 10 og senere versjoner

    Andre nettlesere, for eksempel Google Chrome og Mozilla Firefox, støttes ikke.

- Organisasjonen kan koble til endepunktet i Azure, som er ** \* .blob.core.windows.net** (jokertegnet representerer en unik identifikator for eksportjobben).

- Du tilordnes eksportrollen i Microsoft 365 Security &amp; Compliance Center. Som standard tilordnes denne rollen bare til rollegruppen eDiscovery Manager. Se [Tilordne eDiscovery-tillatelser](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Hvis du vil ha mer informasjon, kan du se [Eksportere søkeresultater for innhold](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).
  