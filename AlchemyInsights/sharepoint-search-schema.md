---
title: Behandle søke skjema i SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770560"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="16a70-102">Behandle søke skjema i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="16a70-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="16a70-103">Søke skjemaet kontrollerer hva brukere kan søke etter, hvordan brukere kan søke i det, og hvordan du kan presentere resultatene på søke nett stedene.</span><span class="sxs-lookup"><span data-stu-id="16a70-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="16a70-104">Se [Behandle søke skjemaet i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) for å lære hvordan du kan gjøre følgende:</span><span class="sxs-lookup"><span data-stu-id="16a70-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="16a70-105">Endre søke skjemaet.</span><span class="sxs-lookup"><span data-stu-id="16a70-105">Change the search schema.</span></span>
- <span data-ttu-id="16a70-106">Opprette forvaltede egenskaper.</span><span class="sxs-lookup"><span data-stu-id="16a70-106">Create managed properties.</span></span>
- <span data-ttu-id="16a70-107">Tilordne krav Les økte egenskaper i tilknytning til forvaltede egenskaper.</span><span class="sxs-lookup"><span data-stu-id="16a70-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="16a70-108">Vær oppmerksom på følgende når du skal håndtere søke skjemaet:</span><span class="sxs-lookup"><span data-stu-id="16a70-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="16a70-109">Hvis du får en advarsel som sier **at programmet er stanset midlertidig** når du foretar en skjema endring, er dette bare midlertidig siden det oppstår service vedlikehold.</span><span class="sxs-lookup"><span data-stu-id="16a70-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="16a70-110">Hvis det har gått mer enn 24 timer og du fremdeles opplever advarselen, kan du logge en støtte sak.</span><span class="sxs-lookup"><span data-stu-id="16a70-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="16a70-111">Når du endrer forvaltede egenskaper eller legger til nye, trer endringene i kraft bare etter at innholdet har blitt krav Les økt på nytt.</span><span class="sxs-lookup"><span data-stu-id="16a70-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="16a70-112">I SharePoint Online skjer automatisk kravlesøk basert på den definerte tids planen for kravlesøk.</span><span class="sxs-lookup"><span data-stu-id="16a70-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="16a70-113">Hvis du vil forsikre deg om at endringene dine er krav Les økt, kan du spesifikt [be om en ny indeksering av listen eller biblioteket](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="16a70-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="16a70-114">Hvis du vil ha en fullstendig oversikt over søke skjemaet, kan du se [innføring i søke skjema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="16a70-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


