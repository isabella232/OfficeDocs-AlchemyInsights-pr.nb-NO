---
title: 'samme som filnavnet er best [REGEL #-beskrivelse]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 1bb1cb35f06e16a2dc85b7e2642b9fa0d203945e
ms.sourcegitcommit: b032c2ac45540b1eb5dd68a4ec7ce1a5d6922f0e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662939"
---
# <a name="required-customer-facing-h1-h2-doesnt-work"></a>Nødvendige kunden motstående H1, H2 fungerer ikke
Eksempeltekst blokker - Følg disse instruksjonene:

1. Filene i mappen **AlchemyInsights** skal ha regel-ID og navn på regel fra [Alkymi partnerportal](https://alchemyportal.azurewebsites.net) i filnavnet.
    1. f.eks. ***976-How-to-enable-litigation-hold***
1. Bruke metadata på toppen av denne filen som malen. Ikke noe annet er nødvendig.
1. Naviger ned til delen i [Alkymi partnerportal](https://alchemyportal.azurewebsites.net) **kunden innsikt tittel:** og bruk som starter en peker for H1 tittelen for innsikt. 
    > [!NOTE]
    > Alkymi Insights må bare en enkelt H1 øverst eller de brytes i produksjon. H2s gjengis ikke så Bruk **fet** eller andre konvensjoner på separate deler.
1. Deretter fyller du ut brødtekst med kladd-materiale i kunden Insights-delen av siden Alkymi regel
    1. Punktmerkede lister er greit
    1. Nummererte lister for
    1. **Fet** og *kursiv* er a-ok
    1. Koblinger må alltid være enten **"koblinger til Web-område" / ekstern** eller **dyp-koblinger til grensesnittelementene**, ikke interne koblinger.

Og dette er virkelig allerede litt for langt. Beste praksis er omtrent 400 tegn---

Når innholdet er klar, drar du den til live grenen. Deretter kan du gå til [partnerportalen på Alkymi](https://alchemyportal.azurewebsites.net) og skriver inn filnavnet i feltet URL-adresse. Kontroller at innsikt gjennomgått og publisert sier "Ja", og klikk deretter Oppdateringsregelen. (Dette ser prettier i den nye versjonen av portalen - slippe snart.)

![URL-adresse-feltet](media/for-content-team.PNG)

