---
title: Bruke Microsoft Edge basert på Chromium nettlesere for Ediscovery-eksport
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
ms.openlocfilehash: a583896b5aa8e73be5e932a729c380acc8092e73b2151647c999f9a7b69669b6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998403"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>Bruke Microsoft Edge basert på Chromium nettlesere for Ediscovery-eksport

På grunn av en nylig endring vil Microsoft Edge nettlesere ikke lenger ha ClickOnce aktivert som standard. Hvis du vil fortsette å Microsoft 365 eDiscovery-eksportverktøyet, må du enten bruke Microsoft Internet Explorer eller aktivere ClickOnce kundestøtte i Microsoft Edge. 

Slik aktiverer ClickOnce støtte i Microsoft Edge basert på Chromium: 
1. Gå til Microsoft Edge i edge://flags/#edge-click-once nettleseren.
2. Endre verdien ClickOnce Standard eller Deaktivert  **til** Aktivert for alternativet for ClickOnce **kundestøtte.** 
3. Velg Start på nytt nederst i **nettleservinduet.** <br>
 Endringen trer i kraft etter at du har startet Microsoft Edge. 

Hvis du vil ha informasjon om dette og fremgangsmåten for å installere eksportverktøyet, kan du se: [ Eksportere søkeresultater for innhold](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).