---
title: Bruke Microsoft Edge basert på Chromium-nettlesere for Ediscovery-eksport
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
- "3473"
- "3100022"
ms.openlocfilehash: 7ee724e5109effce8883be50e360948313c84b34
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834380"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>Bruke Microsoft Edge basert på Chromium-nettlesere for Ediscovery-eksport

På grunn av en nylig endring vil ikke Microsoft Edge-nettlesere lenger ha ClickOnce-støtte aktivert som standard. Hvis du vil fortsette å bruke microsoft 365 eDiscovery-eksportverktøyet, må du enten bruke Microsoft Internet Explorer eller aktivere ClickOnce-støtte i Microsoft Edge. 

Slik aktiverer du ClickOnce-støtte i Microsoft Edge basert på Chromium: 
1. Gå til Edge://flags/#edge-click-once i Microsoft Edge-nettleseren.
2. For alternativet ClickOnce Support endrer du verdien fra **Standard** eller **Deaktivert** til **Aktivert**. 
3. Velg Start på nytt nederst i **nettleservinduet.** <br>
 Endringen trer i kraft etter at du har startet Microsoft Edge på nytt. 

Hvis du vil ha informasjon om dette og fremgangsmåten for å installere eksportverktøyet, kan du se: [ Eksportere søkeresultater for innhold](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).