---
title: Innhold vises ikke i søke resultater i SharePoint
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
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713139"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Innhold vises ikke i søke resultater i SharePoint

Følg disse feil søkings trinnene når forventet innhold ikke vises i søke resultatene:
  
1. Kontroller at **området** som inneholder det forventede innholdet, er satt til å tillate at innhold vises i søke resultatene. Følg Fremgangs måten i [vise innhold på et område i søke resultater](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Kontroller at **listen** eller **biblioteket** som inneholder det forventede innholdet, er satt til å tillate at innhold vises i søke resultatene. Følg Fremgangs måten i [vise innhold fra lister eller biblioteker i søke resultater](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Kontroller at siden, dokumentet eller egen definert side oppsett publiseres som **hovedversjon.** Følg trinn 3 i [Søk returnerer ikke alle resultatene i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Kontroller at brukeren har **tillatelse** til å vise innholdet. Følg Fremgangs måten i [forstå tillatelses nivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Hvis søke skjemaet er endret ved å legge til en ny forvaltet egenskap, ved å redigere en forvaltet egenskap eller ved å fjerne en forvaltet egenskap, må du be om et kravlesøk og reindekse. **Indekser** innholdet på nytt ved å følge trinnene i [manuelt be om kravlesøk og indeksering av et nettsted, et bibliotek eller en liste](https://docs.microsoft.com/sharepoint/crawl-site-content). Dette kan ta litt tid å vente i 24 timer før du ser resultatene på nytt.

Hvis du vil ha mer informasjon, kan du se [aktivere innhold på et nettsted for å bli søkbart](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
