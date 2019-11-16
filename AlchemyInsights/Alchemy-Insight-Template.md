---
title: samme som filnavn er best
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
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/15/2019
ms.locfileid: "35800054"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Krevde alkymi overskriften H1, H2's dont ' arbeide.
Best Practices og retningslinjer for Alchemy authoring:

1. **Ikke hekker Alchemy Insights i mapper**-dette vil bryte URL strukturen. Vi ser på å fikse dette.
1. Filer i mappen **AlchemyInsights** bør ha små filnavn med bindestreker for mellomrom. ***hvordan-å-aktivere-søksmål-Hold***.
    1. Inkluder regel-ID eller Bucket ID fra [Alchemy partner-portalen](https://alchemyportal.azurewebsites.net) i det egendefinerte feltet MS. Ex. ***MS Custom: 100021***
1. Bruk resten av metadataene øverst i denne filen som mal.
1. I [Alchemy partner Portal](https://alchemyportal.azurewebsites.net), Naviger ned til seksjonen **Customer Insight tittel:** og bruke det som et utgangspunkt for H1 tittel for innsikt. 
    > [!NOTE]
    > Alchemy Insights må ha bare en enkelt H1 på toppen eller de vil bryte i produksjon. H2s ikke gjengi enten så bruk **fet** eller andre konvensjoner for å betegne separate seksjoner.
1. Deretter fyller du ut brødteksten ved hjelp av kladde materialet i delen Kundeinnsikt på siden alkymi-regel
    1. Punktmerkede lister er fine
    1. Nummererte lister også
    1. **Fet** og *kursiv* er en-OK
    1. Linker bør alltid være enten **"lenker til Web"/External** eller **Deep-linker til UI elementer**, ikke interne koblinger.
    1. Bilder er ikke offisielt støttet på dette tidspunktet, men det er på veikart.

Og dette er egentlig allerede litt for lang. Beste praksis er om 400 tegn---------------------------------

Når innholdet er klart, drar du det til den aktive grenen. Deretter går du til [alkymi partner portalen](https://alchemyportal.azurewebsites.net) og skriv inn filnavnet i URL-feltet. 