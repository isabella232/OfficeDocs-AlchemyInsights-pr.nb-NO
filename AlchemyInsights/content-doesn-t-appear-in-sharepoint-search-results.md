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
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="38464-102">Innhold vises ikke i SharePoint-søkeresultater</span><span class="sxs-lookup"><span data-stu-id="38464-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="38464-103">Følg disse feilsøkingstrinnene når forventet innhold ikke vises i søkeresultatene:</span><span class="sxs-lookup"><span data-stu-id="38464-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="38464-104">Kontroller at **området** som inneholder det forventede innholdet, er satt til å tillate at innhold vises i søkeresultatene.</span><span class="sxs-lookup"><span data-stu-id="38464-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="38464-105">Følg trinnene i [Vis innhold på et nettsted i søkeresultatene](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="38464-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="38464-106">Kontroller at **listen** eller **biblioteket** som inneholder det forventede innholdet, er satt til å tillate at innhold vises i søkeresultatene.</span><span class="sxs-lookup"><span data-stu-id="38464-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="38464-107">Følg trinnene i [Vis innhold fra lister eller biblioteker i søkeresultatene](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="38464-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="38464-108">Kontroller at side-, dokument- eller egendefinertsideoppsettet er publisert som en **hovedversjon.**</span><span class="sxs-lookup"><span data-stu-id="38464-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="38464-109">Følg trinn 3 i [Søk returnerer ikke alle resultater i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="38464-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="38464-110">Kontroller at brukeren har **tillatelse** til å vise innholdet.</span><span class="sxs-lookup"><span data-stu-id="38464-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="38464-111">Følg trinnene i [Forstå tillatelsesnivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="38464-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="38464-112">Hvis søkeskjemaet er endret ved å legge til en ny forvaltet egenskap, ved å redigere en forvaltet egenskap eller ved å fjerne en forvaltet egenskap, må det være nødvendig med en kravlesøk og re-indeks.</span><span class="sxs-lookup"><span data-stu-id="38464-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="38464-113">**Indekser** innholdet på nytt ved å følge trinnene i [Be om kravlesøk og indeksering på nytt for et område, et bibliotek eller en liste](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="38464-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="38464-114">Dette kan ta en stund, vent 24 timer før du sjekker resultatene igjen.</span><span class="sxs-lookup"><span data-stu-id="38464-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="38464-115">Hvis du vil ha mer informasjon, kan du se [Aktivere innhold på et område for å være søkbart](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="38464-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
