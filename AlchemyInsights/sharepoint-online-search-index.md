---
title: Søk i SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507640"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Innhold på kravlesøk og indeksering i SharePoint Online

Innhold må være kravlesøkt og lagt til i søkeindeksen for brukerne å finne det de søker etter i SharePoint Online. Innhold kravlesøkes automatisk basert på en forhåndsdefinert kravlesøk tidsplan (tidsplan for kravlesøk ikke kan endres). Kravlesøkeren plukker opp innhold som er endret siden sist kravlesøk og oppdaterer indeksen. For å sikre innhold kravlesøkes og indeksen oppdateres, Vær oppmerksom på følgende:

- Pass på at du finner innhold ved [å gjøre innhold søkbart](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Når du har endret en forvaltet egenskap, eller når du har endret tilordning av kravlesøkt og administreres må, området være kravlesøkt på nytt før endringene gjenspeiles i søkeindeksen. 

    Fordi endringene er gjort i søkeskjemaet, og ikke til det faktiske området, vil søkemotoren ikke automatisk indeksere området på nytt. 

    For mer informasjon, se [Be om kravlesøk og indeksering på nytt på et område, et bibliotek eller en liste manuelt](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Vent minst 24 timer etter manuelt ber om et kravlesøk og full indeksere på nytt for å se om du fremdeles har et problem. 

    Hvis det har gått mer enn 24 timer etter at du startet kravlesøk og full indeksere på nytt, logger du deg en sak for støtte. I mange tilfeller kan arbeider vi allerede med en løsning. Gi oss minst 24 timer å fullføre en løsning.

> [!IMPORTANT]
> Hvis et område (bibliotek)-dokument eller en liste ble slettet og fremdeles i søkeresultatene, brukere som skal motta en **Feil 404 Finner ikke filen** når du prøver å få tilgang til den. Dette problemet bør være logget som en støtte sak for videre undersøkelse. 



