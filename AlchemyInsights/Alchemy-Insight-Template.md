---
title: det samme som filnavnet er best
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312834"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Required Alchemy Header H1, H2's don's don't work."
Anbefalte fremgangsmåter og retningslinjer for Alchemy-redigering:

1. **Ikke neste Alchemy Insights i mapper**– dette vil bryte url-strukturen. Vi jobber med å løse dette.
1. Filer i **Mappen AlchemyInsights** skal ha små filnavn med bindestreker for mellomrom f.eks. **_how-to-enable-litigation-hold_**.
    1. Inkluder regel-ID-en eller samlings-ID-en fra [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net) i ms.custom-feltet. f.eks. ***ms.custom: 100021***
1. Bruk resten av metadataene øverst i denne filen som mal.
1. Naviger ned til delen Customer **Insight Title** i [Alchemy Partner-portalen,](https://alchemyportal.azurewebsites.net)og bruk den som utgangspunkt for H1-tittelen for innsikten. 

**Obs!** Alchemy Insights MÅ bare ha én enkelt H1 øverst, ellers vil de brytes i produksjon. H2-er gjengis ikke, så bruk **fet** eller andre konvensjoner til å betegne separate inndelinger.
1. Deretter fyller du ut brødteksten ved hjelp av kladdematerialet i Customer Insights på alkymiregelsiden
    1. Punktlister er i orden
    1. Nummererte lister også
    1. **Fet** og *kursiv* er a-ok
    1. Koblinger bør alltid være **enten koblinger til nettet/eksterne** ELLER dypkoblinger til **grensesnittelementer,** ikke interne koblinger.
    1. Bilder støttes for øyeblikket ikke offisielt, men det er på veikartet.

Og dette er egentlig allerede litt for langt. Beste fremgangsmåte er omtrent 400 tegn ---------------------------------

Når innholdet er klart, drar du det til den direkte grenen. Deretter går du til [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net) og skriver inn filnavnet i nettadressefeltet. 