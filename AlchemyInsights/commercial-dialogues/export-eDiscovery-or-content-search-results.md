---
title: Eksportere søkeresultater for eDiscovery/innholdssøk
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7221"
ms.openlocfilehash: de5d6f2bbf32ca1b7a0bbb9dd416fb19186d2e72ad57fbf25d9b55bd733fdc21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988122"
---
# <a name="export-ediscoverycontent-search-results"></a>Eksportere søkeresultater for eDiscovery/innholdssøk

Du må kanskje eksportere søkeresultatene til en PST-fil (fra e-post) eller til opprinnelige Office dokumenter (fra SharePoint og OneDrive for Business nettsteder). Hvis dette er det, gjør du følgende:

- Kontroller at kontoen er tilordnet de riktige tillatelsene til å eksportere. Hvis du vil ha mer informasjon, kan du se [Tilordne eDiscovery-tillatelse](https://go.microsoft.com/fwlink/?linkid=2102406).
- Kontroller at datamaskinen har oppfylt [alle forutsetninger.](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin) Ikke alle nettlesere støttes, for eksempel Chrome.
- Slik eksporterer du fra et innholdssøk: a. Gå til [sikkerhetssenteret & samsvarssenteret,](https://protection.office.com/contentsearch) og klikk **Søk**, og velg deretter **Innholdssøk**. Velg et **lagret søk** på Innholdssøk-siden.
    b. Velg Start eksport under **Eksporter resultater til en datamaskin** i **Detalj-ruten.** Hvis du eksporterer mer enn 100 000 postbokser, må du bruke PowerShell til å laste ned eksportresultatene. Hvis du vil ha mer informasjon, [kan du se Eksportere resultater fra mer enn 100 000 postbokser](https://go.microsoft.com/fwlink/?linkid=2143861).

Hvis du vil ha mer informasjon, [kan du se Eksportere søkeresultater for innhold](https://go.microsoft.com/fwlink/?linkid=2102118).