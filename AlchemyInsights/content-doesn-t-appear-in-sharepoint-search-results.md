---
title: Innhold vises ikke i SharePoint-søkeresultater
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705670"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Innhold vises ikke i SharePoint-søkeresultater

Følg disse feilsøkingstrinnene når forventet innhold ikke vises i søkeresultatene:
  
1. Kontroller at **området** som inneholder det forventede innholdet, er satt til å tillate at innhold vises i søkeresultatene. Følg trinnene i [Vis innhold på et nettsted i søkeresultatene](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Kontroller at **listen** eller **biblioteket** som inneholder det forventede innholdet, er satt til å tillate at innhold vises i søkeresultatene. Følg trinnene i [Vis innhold fra lister eller biblioteker i søkeresultatene](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Kontroller at side-, dokument- eller egendefinertsideoppsettet er publisert som en **hovedversjon.** Følg trinn 3 i [Søk returnerer ikke alle resultater i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Kontroller at brukeren har **tillatelse** til å vise innholdet. Følg trinnene i [Forstå tillatelsesnivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Hvis søkeskjemaet er endret ved å legge til en ny forvaltet egenskap, ved å redigere en forvaltet egenskap eller ved å fjerne en forvaltet egenskap, må det være nødvendig med en kravlesøk og re-indeks. **Indekser** innholdet på nytt ved å følge trinnene i [Be om kravlesøk og indeksering på nytt for et område, et bibliotek eller en liste](https://docs.microsoft.com/sharepoint/crawl-site-content). Dette kan ta en stund, vent 24 timer før du sjekker resultatene igjen.

Hvis du vil ha mer informasjon, kan du se [Aktivere innhold på et område for å være søkbart](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
