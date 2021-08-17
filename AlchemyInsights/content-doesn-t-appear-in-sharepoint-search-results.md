---
title: Innhold vises ikke i SharePoint søkeresultater
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081619"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Innhold vises ikke i SharePoint søkeresultater

Følg disse feilsøkingstrinnene når forventet innhold ikke vises i søkeresultatene:
  
1. Kontroller at nettstedet **som** inneholder det forventede innholdet, er satt til å tillate at innhold vises i søkeresultatene. Følg fremgangsmåten i [Vise innhold på et nettsted i søkeresultater](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Kontroller at listen **eller** **biblioteket som** inneholder det forventede innholdet, er satt til å tillate at innhold vises i søkeresultatene. Følg fremgangsmåten i [Vise innhold fra lister eller biblioteker i søkeresultater](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Kontroller at siden, dokumentet eller det egendefinerte sideoppsettet er publisert som en **hovedversjon.** Følg trinn 3 i [Søk returnerer](https://go.microsoft.com/fwlink/?linkid=874525)ikke alle resultatene i SharePoint Online .

4. Kontroller at brukeren har **tillatelse til** å vise innholdet. Følg fremgangsmåten i [Forstå tilgangsnivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Hvis søkeskjemaet er endret ved å legge til en ny forvaltet egenskap, ved å redigere en forvaltet egenskap eller ved å fjerne en forvaltet egenskap, kreves det kravlesøk og ny indeks. **Indekser innholdet på** nytt ved å følge trinnene i Be om kravlesøk og indeksering på nytt for et [nettsted, et bibliotek eller en liste.](https://docs.microsoft.com/sharepoint/crawl-site-content) Dette kan ta litt tid, vent 24 timer før du kontrollerer resultatene på nytt.

Hvis du vil ha mer informasjon, kan du se Aktivere [innhold på et nettsted for å være søkbart](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
