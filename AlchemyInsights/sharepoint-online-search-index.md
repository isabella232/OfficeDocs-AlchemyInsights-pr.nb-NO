---
title: Søk i SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: fc49978fbd2c07381dae83061b1a1868cd1df0d0
ms.sourcegitcommit: 327a2c77afc2ff3d67d3aaaea1a92068a3c4bb1f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/06/2019
ms.locfileid: "36059261"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="0c1bc-102">Søk i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="0c1bc-102">Search in SharePoint Online</span></span>

<span data-ttu-id="0c1bc-103">Innhold må være kravlesøkt og lagt til i søkeindeksen for brukerne å finne det de søker etter i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="0c1bc-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="0c1bc-104">Innhold kravlesøkes automatisk basert på en forhåndsdefinert kravlesøk tidsplan (tidsplan for kravlesøk ikke kan endres).</span><span class="sxs-lookup"><span data-stu-id="0c1bc-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="0c1bc-105">Kravlesøkeren plukker opp innhold som er endret siden sist kravlesøk og oppdaterer indeksen.</span><span class="sxs-lookup"><span data-stu-id="0c1bc-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="0c1bc-106">For å sikre innhold kravlesøkes og indeksen oppdateres, Vær oppmerksom på følgende:</span><span class="sxs-lookup"><span data-stu-id="0c1bc-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="0c1bc-107">Pass på at du finner innhold ved [å gjøre innhold søkbart](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="0c1bc-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="0c1bc-108">Når du har endret en forvaltet egenskap, eller når du har endret tilordning av kravlesøkt og administreres må, området være kravlesøkt på nytt før endringene gjenspeiles i søkeindeksen.</span><span class="sxs-lookup"><span data-stu-id="0c1bc-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="0c1bc-109">Fordi endringene er gjort i søkeskjemaet, og ikke til det faktiske området, vil søkemotoren ikke automatisk indeksere området på nytt.</span><span class="sxs-lookup"><span data-stu-id="0c1bc-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="0c1bc-110">For mer informasjon, se [Be om kravlesøk og indeksering på nytt på et område, et bibliotek eller en liste manuelt](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="0c1bc-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="0c1bc-111">Vent minst 24 timer etter manuelt ber om et kravlesøk og full indeksere på nytt for å se om du fremdeles har et problem.</span><span class="sxs-lookup"><span data-stu-id="0c1bc-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="0c1bc-112">Hvis det har gått mer enn 24 timer etter at du startet kravlesøk og full indeksere på nytt, logger du deg en sak for støtte.</span><span class="sxs-lookup"><span data-stu-id="0c1bc-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="0c1bc-113">I mange tilfeller kan arbeider vi allerede med en løsning.</span><span class="sxs-lookup"><span data-stu-id="0c1bc-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="0c1bc-114">Gi oss minst 24 timer å fullføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="0c1bc-114">Please give us at least 24 hours to complete a solution.</span></span>

>[! Viktig!]<span data-ttu-id="0c1bc-115">: Hvis et område, (bibliotek)-dokument eller en liste ble slettet og fortsatt vises i søkeresultatene, brukere skal motta en **Feil 404 Finner ikke filen** når du prøver å få tilgang til den.</span><span class="sxs-lookup"><span data-stu-id="0c1bc-115">: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="0c1bc-116">Dette problemet bør være logget som en støtte sak for videre undersøkelse.</span><span class="sxs-lookup"><span data-stu-id="0c1bc-116">This issue should be logged as a support case for further investigation.</span></span> 



