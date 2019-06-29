---
title: Innhold vises ikke i søkeresultatene for SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: 8215b0a5cde5adffa3bec37d6699418557f914dd
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363824"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Innhold vises ikke i søkeresultatene for SharePoint

Følg disse feilsøkingstrinnene når forventet innhold ikke vises i søkeresultatene:
  
1. Kontroller at **området** som inneholder det forventede innholdet er satt til å tillate at innhold skal vises i søkeresultatene. Følg trinnene i [Vis innhold på et område i søkeresultatene](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Kontroller at **listen** eller **biblioteket** som inneholder det forventede innholdet er satt til å tillate at innholdet vises i søkeresultatene. Følg trinnene i [Vis innhold fra listene eller bibliotekene i søkeresultatene](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Kontroller at siden, dokumentet eller egendefinerte sideoppsett er publisert som en **hovedversjon.** Følg instruksjonene i trinn 3 i [Søk returnerer ikke alle resultatene i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Kontroller at brukeren har **tillatelser** til å vise innholdet. Følg trinnene i [Forstå tillatelsesnivåer i SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).
    
5. Hvis søkeskjemaet har blitt endret ved å legge til en ny forvaltet egenskap, ved å redigere en forvaltet egenskap, eller ved å fjerne en forvaltet egenskap deretter ber du om et kravlesøk, og vil være nødvendig å indeksere på nytt. **Reindekser** innholdet ved å følge trinnene i [forespørsel manuelt på kravlesøk og indeksering på nytt på et område, et bibliotek eller en liste](https://docs.microsoft.com/sharepoint/crawl-site-content). Dette kan ta litt tid, vente 24 timer før du kontrollerer resultatene på nytt.

Hvis du vil ha mer informasjon, kan du se [aktivere innholdet på et område skal være søkbare](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
