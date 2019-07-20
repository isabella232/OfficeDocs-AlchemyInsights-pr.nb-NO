---
title: samme som filnavnet er best
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800054"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Nødvendig Alkymi hodet H1, H2's virker ikke.
Gode fremgangsmåter og retningslinjer for redigering av Alkymi:

1. **Ikke nest Alkymi innsikt i mapper**- dette vil bryte URL-strukturen. Vi er ute til å fikse dette.
1. Filene i mappen **AlchemyInsights** skal ha små bokstaver filnavn med bindestreker for mellomrom ex. ***how-skal aktivere-rettstvist-Vent***.
    1. Ta med regel-ID eller bucket ID fra [Alkymi partnerportal](https://alchemyportal.azurewebsites.net) i feltet ms.custom. EX. ***MS.Custom: 100021***
1. Bruk resten av metadataene på toppen av denne filen som malen.
1. Naviger ned til delen i [Alkymi partnerportal](https://alchemyportal.azurewebsites.net) **kunden innsikt tittel:** og bruk som starter en peker for H1 tittelen for innsikt. 
    > [!NOTE]
    > Alkymi Insights må bare en enkelt H1 øverst eller de brytes i produksjon. H2s gjengis ikke så Bruk **fet** eller andre konvensjoner på separate deler.
1. Deretter fyller du ut brødtekst med kladd-materiale i kunden Insights-delen av siden Alkymi regel
    1. Punktmerkede lister er greit
    1. Nummererte lister for
    1. **Fet** og *kursiv* er a-ok
    1. Koblinger må alltid være enten **"koblinger til Web-område" / ekstern** eller **dyp-koblinger til grensesnittelementene**, ikke interne koblinger.
    1. Bilder offisielt støtter ikke denne gangen, men det er på veikartet for tiltaket.

Og dette er virkelig allerede litt for langt. Beste praksis er omtrent 400 tegn---

Når innholdet er klar, drar du den til live grenen. Deretter kan du gå til [partnerportalen på Alkymi](https://alchemyportal.azurewebsites.net) og skriver inn filnavnet i feltet URL-adresse. 