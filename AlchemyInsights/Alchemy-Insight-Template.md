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
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750979"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Krevde Alkymi Header H1, H2's fungerer ikke."
Beste praksis og retningslinjer for alkymiredigering:

1. **Ikke nest Alchemy Insights i mapper**- dette vil bryte url-strukturen. Vi undersøker dette.
1. Filer i **AlchemyInsights-mappen** bør ha små bokstaver med bindestreker for mellomrom ex. ***how-to-enable-litigation-hold***.
    1. Inkluder regel-ID-en eller bucket-ID-en fra [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net) i ms.custom-feltet. Ex. ***ms.custom: 100021***
1. Bruk resten av metadataene øverst i denne filen som mal.
1. I [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net)navigerer du ned til delen **Customer Insight-tittel,** og bruker det som utgangspunkt for H1-tittelen for innsikten. 
    > [!NOTE]
    > Alchemy Insights MÅ ha bare en enkelt H1 på toppen, eller de vil bryte i produksjon. H2s gjengis ikke, så bruk **fet eller** andre konvensjoner for å betegne separate deler.
1. Deretter fyller du ut brødteksten ved hjelp av kladdematerialet i Kundeinnsikt-delen på Alchemy Rule-siden
    1. Punktlister er fine
    1. Nummererte lister også
    1. **Fet** og *kursiv* er a-ok
    1. Lenker bør alltid være **enten "lenker til web"/eksterne** ELLER **dypkoblinger til UI-elementer**, ikke interne koblinger.
    1. Bilder støttes ikke offisielt på dette tidspunktet, men det er på veikartet.

Og dette er egentlig allerede litt for lenge. Beste praksis er ca 400 tegn ---------------------------------

Når innholdet er klart, trekker du det til den aktive grenen. Deretter går du til [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net) og skriver inn filnavnet i url-feltet. 