---
title: Behandle søkeskjemaet i SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 704fb3b682d23220d61192e383d7d80f59f27933
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502816"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="aeed0-102">Behandle søkeskjemaet i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="aeed0-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="aeed0-103">Søkeskjemaet kontrollerer hva brukere kan søke etter, hvor brukere kan søke, og hvordan du kan presentere resultatene på Søk-webområder.</span><span class="sxs-lookup"><span data-stu-id="aeed0-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="aeed0-104">Se [Behandle søkeskjemaet i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) til å lære hvordan du:</span><span class="sxs-lookup"><span data-stu-id="aeed0-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="aeed0-105">Endre søkeskjemaet.</span><span class="sxs-lookup"><span data-stu-id="aeed0-105">Change the search schema.</span></span>
- <span data-ttu-id="aeed0-106">Lage forvaltede egenskaper.</span><span class="sxs-lookup"><span data-stu-id="aeed0-106">Create managed properties.</span></span>
- <span data-ttu-id="aeed0-107">Tilordne kravlesøkte kart kravlesøkte egenskaper til forvaltede egenskaper.</span><span class="sxs-lookup"><span data-stu-id="aeed0-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="aeed0-108">Vær oppmerksom på følgende når det gjelder administrasjon av Search-skjema:</span><span class="sxs-lookup"><span data-stu-id="aeed0-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="aeed0-109">Hvis du får en advarsel om **programmet er midlertidig stanset** når du foretar en skjemaendring i XML-, dette er bare midlertidige som maintenance service som forekommer.</span><span class="sxs-lookup"><span data-stu-id="aeed0-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="aeed0-110">Hvis det har gått mer enn 24 timer, og du fortsatt opplever advarselen, Logg en sak for støtte.</span><span class="sxs-lookup"><span data-stu-id="aeed0-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="aeed0-111">Når du endrer forvaltede egenskaper, eller legge til nye, trer endringene i kraft bare etter at innholdet er kravlesøkt på nytt.</span><span class="sxs-lookup"><span data-stu-id="aeed0-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="aeed0-112">I SharePoint Online skjer kravlesøk automatisk basert på tidsplan for definerte kravlesøk.</span><span class="sxs-lookup"><span data-stu-id="aeed0-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="aeed0-113">Hvis du vil forsikre deg om at endringene blir kravlesøkt, kan du spesifikt [Be om et nytt indeksering av listen eller biblioteket](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="aeed0-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="aeed0-114">For en fullstendig oversikt over søkeskjemaet, se [Innføring i søkeskjemaet](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="aeed0-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


