---
title: samme som fil navnet er best
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
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664143"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Obligatorisk Alchemy-hode H1, H2's fungerer ikke."
Beste Fremgangs måter og retnings linjer for Alchemy redigering:

1. Ikke **neste Alchemye innsikt i mapper**– dette vil bryte URL-strukturen. Vi er i ferd med å rette opp dette.
1. Filer i **AlchemyInsights** -mappen bør ha små bokstaver med binde streker for mellomrom ex. Fremgangs ***måte for aktivering – retts tvist-vent***.
    1. Inkluder regel-ID-en eller spann-ID-en fra [Alchemy partner Portal](https://alchemyportal.azurewebsites.net) i MS. Custom-feltet. &. ***MS. Custom: 100021***
1. Bruk resten av metadataene øverst i denne filen som mal.
1. I [Alchemy partner portalen](https://alchemyportal.azurewebsites.net)navigerer du ned til inndelingen **kunde innsikt tittel:** og bruker dette som et utgangs punkt for den H1-tittelen for innsiktet. 
    > [!NOTE]
    > Alchemy innsikter må ha bare én enkelt H1 øverst, eller de kommer til å bryte i produksjon. H2s ikke gjengir, så du kan bruke **fet** eller andre konvensjoner til å skille mellom separate inndelinger.
1. Deretter fyller du ut brød teksten ved hjelp av kladde materialet i delen kunde innsikt på Alchemy Regels IDen
    1. Punkt lister er fine
    1. Nummererte lister
    1. **Fet** og *kursiv* er en-OK
    1. Koblinger må alltid være enten **koblinger til Web-/External** eller **dype koblinger til grensesnitt elementer**, ikke interne koblinger.
    1. Bilder støttes ikke offisielt på dette tidspunktet, men det er på vei kartet.

Og dette er faktisk allerede litt for langt. Beste Fremgangs måte er omtrent 400 tegn---------------------------------

Når innholdet er klart, kan du dra det til direkte grenen. Gå deretter til [Alchemy partner Portal](https://alchemyportal.azurewebsites.net) , og skriv inn fil navnet i URL-feltet. 