---
title: samme som filnavn er best
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676542"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Krevde Alchemy Header H1, H2's fungerer ikke.
Beste praksis og retningslinjer for Alkymi redigering:

1. **Ikke neste Alchemy Insights i mapper**- dette vil bryte url strukturen. Vi undersøker dette.
1. Filer i **AlchemyInsights-mappen** bør ha små filnavn med bindestreker for mellomrom ex. ***hvordan-å-aktivere-rettstvist-hold***.
    1. Inkluder regel-ID-en eller samlings-IDen fra [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net) i ms.custom-feltet. Ex. ***ms.custom: 100021***
1. Bruk resten av metadataene øverst i denne filen som mal.
1. I [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net)navigerer du ned til delen **Customer Insight-tittel:** og bruk dette som utgangspunkt for H1-tittelen for innsikten. 
    > [!NOTE]
    > Alchemy Insights MÅ bare ha en enkelt H1 på toppen, ellerde vil bryte i produksjon. H2s ikke gjengi enten så bruk **fet eller** andre konvensjoner for å betegne separate seksjoner.
1. Deretter fyller du ut brødteksten ved hjelp av utkastet til materiale i Kundeinnsikt-delen på Siden Alchemy-regel
    1. Punktlister er fine
    1. Nummererte lister også
    1. **Fet** og *kursiv* er a-ok
    1. Lenker bør alltid være enten **"lenker til web"/eksterne** ELLER **dyplenker til brukerelementer**, ikke interne lenker.
    1. Bilder støttes ikke offisielt på dette tidspunktet, men det er på veikartet.

Og dette er egentlig allerede litt for lenge. Beste praksis er ca 400 tegn ---------------------------------

Når innholdet er klart, trekker du det til den direktesendte grenen. Deretter går du til [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net) og skriver inn filnavnet i url-feltet. 