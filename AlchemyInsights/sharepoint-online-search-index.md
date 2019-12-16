---
title: Søk i SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044052"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Kravlesøk og indeksering av innhold i SharePoint Online

Innhold må kravlesøkes og legges til i søkeindeksen for at brukerne skal kunne finne det de leter etter i SharePoint Online. Innhold kravlesøkes automatisk basert på en forhåndsdefinert tidsplan for kravlesøk (tidsplanen for kravlesøk kan ikke endres). Søkeroboten plukker opp innhold som er endret siden siste kravlesøk, og oppdaterer indeksen. Merk deg følgende for å sikre at innholdet kravlesøkes og indeksen oppdateres:

- Sørg for at innhold kan bli funnet ved [å gjøre innholdet på området søkbart](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Når du har endret en forvaltet egenskap, eller når du har endret tilordningen av kravlesøkte og forvaltede egenskaper, må området kravlesøkes på nytt før endringene gjenspeiles i søkeindeksen. 

    Fordi endringene er gjort i søkeskjemaet, og ikke til det faktiske området, indekserer ikke søkeroboten automatisk på nytt på området. 

    Hvis du vil ha mer informasjon, kan du se [manuelt forespørre kravlesøk etter og indeksering av et område, et bibliotek eller en liste på nytt](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Vent i minst 24 timer etter at du har bedt om en gjennomgang manuelt og full ny indeks for å se om du fortsatt har problemer. 

    Hvis det har gått mer enn 24 timer siden du startet kravlesøket og fullstendig ny indeks, kan du logge en kundestøttesak. I mange tilfeller er vi allerede jobber med en løsning. Vennligst gi oss minst 24 timer for å fullføre en løsning.

> [!IMPORTANT]
> Hvis et område, et dokument (bibliotek) eller en liste ble slettet og fremdeles vises i søkeresultatene, bør brukere få en **feil 404 Finner ikke filen** når den prøver å få tilgang til den. Dette problemet bør logges som en støtte sak for videre undersøkelser. 



