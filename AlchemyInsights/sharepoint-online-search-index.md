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
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="69f76-102">Kravlesøk og indeksering av innhold i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="69f76-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="69f76-103">Innhold må kravlesøkes og legges til i søkeindeksen for at brukerne skal kunne finne det de leter etter i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="69f76-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="69f76-104">Innhold kravlesøkes automatisk basert på en forhåndsdefinert tidsplan for kravlesøk (tidsplanen for kravlesøk kan ikke endres).</span><span class="sxs-lookup"><span data-stu-id="69f76-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="69f76-105">Søkeroboten plukker opp innhold som er endret siden siste kravlesøk, og oppdaterer indeksen.</span><span class="sxs-lookup"><span data-stu-id="69f76-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="69f76-106">Merk deg følgende for å sikre at innholdet kravlesøkes og indeksen oppdateres:</span><span class="sxs-lookup"><span data-stu-id="69f76-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="69f76-107">Sørg for at innhold kan bli funnet ved [å gjøre innholdet på området søkbart](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="69f76-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="69f76-108">Når du har endret en forvaltet egenskap, eller når du har endret tilordningen av kravlesøkte og forvaltede egenskaper, må området kravlesøkes på nytt før endringene gjenspeiles i søkeindeksen.</span><span class="sxs-lookup"><span data-stu-id="69f76-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="69f76-109">Fordi endringene er gjort i søkeskjemaet, og ikke til det faktiske området, indekserer ikke søkeroboten automatisk på nytt på området.</span><span class="sxs-lookup"><span data-stu-id="69f76-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="69f76-110">Hvis du vil ha mer informasjon, kan du se [manuelt forespørre kravlesøk etter og indeksering av et område, et bibliotek eller en liste på nytt](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="69f76-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="69f76-111">Vent i minst 24 timer etter at du har bedt om en gjennomgang manuelt og full ny indeks for å se om du fortsatt har problemer.</span><span class="sxs-lookup"><span data-stu-id="69f76-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="69f76-112">Hvis det har gått mer enn 24 timer siden du startet kravlesøket og fullstendig ny indeks, kan du logge en kundestøttesak.</span><span class="sxs-lookup"><span data-stu-id="69f76-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="69f76-113">I mange tilfeller er vi allerede jobber med en løsning.</span><span class="sxs-lookup"><span data-stu-id="69f76-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="69f76-114">Vennligst gi oss minst 24 timer for å fullføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="69f76-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="69f76-115">Hvis et område, et dokument (bibliotek) eller en liste ble slettet og fremdeles vises i søkeresultatene, bør brukere få en **feil 404 Finner ikke filen** når den prøver å få tilgang til den.</span><span class="sxs-lookup"><span data-stu-id="69f76-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="69f76-116">Dette problemet bør logges som en støtte sak for videre undersøkelser.</span><span class="sxs-lookup"><span data-stu-id="69f76-116">This issue should be logged as a support case for further investigation.</span></span> 



