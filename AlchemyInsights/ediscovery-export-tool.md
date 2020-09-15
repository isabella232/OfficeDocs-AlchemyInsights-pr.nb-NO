---
title: eksport verktøy for eDiscovery
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 55f29fae0878917eaf2972ba1dfd3c5b8a26ce54
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711104"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kan du ikke installere eller kjøre eksport verktøyet for eDiscovery?

Hvis du ikke kan installere eller kjøre eksport verktøyet for eDiscovery for å laste ned søke resultater, kontrollerer du følgende:
  
- Data maskinen du bruker, oppfyller disse forhånds kravene:

  - 32-eller 64-biters versjoner av Windows 7 og nyere versjoner

  - Microsoft .NET Framework 4.7

  - En støttet nett leser:

  - Microsoft Edge

    eller

  - Internet Explorer 10 og nyere versjoner

    Andre nett lesere, for eksempel Google Chrome og Mozilla Firefox, støttes ikke.

- Organisasjonen kan koble til ende punktet i Azure, som er ** \* . blob.Core.Windows.net** (Joker tegnet representerer en unik identifikator for eksport jobben).

- Du er tilordnet eksport rollen i sikkerhets &amp; samsvars senteret for Microsoft 365. Som standard tilordnes denne rollen bare til rolle gruppen for eDiscovery-ansvarlige. Se [Tilordne eDiscovery-tillatelser](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Hvis du vil ha mer informasjon, kan du se [eksportere søke resultater for innhold](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).
  