---
title: 'samme som filnavnet er best [REGEL #-beskrivelse]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634513"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="24a0c-102">Nødvendig Alkymi hodet H1, H2's virker ikke.</span><span class="sxs-lookup"><span data-stu-id="24a0c-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="24a0c-103">Gode fremgangsmåter og retningslinjer for redigering av Alkymi:</span><span class="sxs-lookup"><span data-stu-id="24a0c-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="24a0c-104">**Ikke nest Alkymi innsikt i mapper**- dette vil bryte URL-strukturen.</span><span class="sxs-lookup"><span data-stu-id="24a0c-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="24a0c-105">Vi er ute til å fikse dette.</span><span class="sxs-lookup"><span data-stu-id="24a0c-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="24a0c-106">Filene i mappen **AlchemyInsights** skal ha regel-ID og navn på regel fra [Alkymi partnerportal](https://alchemyportal.azurewebsites.net) i filnavnet.</span><span class="sxs-lookup"><span data-stu-id="24a0c-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="24a0c-107">EX.</span><span class="sxs-lookup"><span data-stu-id="24a0c-107">ex.</span></span> <span data-ttu-id="24a0c-108">***976-How-to-enable-litigation-Hold***</span><span class="sxs-lookup"><span data-stu-id="24a0c-108">***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="24a0c-109">Bruke metadata på toppen av denne filen som malen.</span><span class="sxs-lookup"><span data-stu-id="24a0c-109">Use the metadata at the top of this file as your template.</span></span> <span data-ttu-id="24a0c-110">Ikke noe annet er nødvendig.</span><span class="sxs-lookup"><span data-stu-id="24a0c-110">Nothing else is required.</span></span>
1. <span data-ttu-id="24a0c-111">Naviger ned til delen i [Alkymi partnerportal](https://alchemyportal.azurewebsites.net) **kunden innsikt tittel:** og bruk som starter en peker for H1 tittelen for innsikt.</span><span class="sxs-lookup"><span data-stu-id="24a0c-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="24a0c-112">Alkymi Insights må bare en enkelt H1 øverst eller de brytes i produksjon.</span><span class="sxs-lookup"><span data-stu-id="24a0c-112">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="24a0c-113">H2s gjengis ikke så Bruk **fet** eller andre konvensjoner på separate deler.</span><span class="sxs-lookup"><span data-stu-id="24a0c-113">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="24a0c-114">Deretter fyller du ut brødtekst med kladd-materiale i kunden Insights-delen av siden Alkymi regel</span><span class="sxs-lookup"><span data-stu-id="24a0c-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="24a0c-115">Punktmerkede lister er greit</span><span class="sxs-lookup"><span data-stu-id="24a0c-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="24a0c-116">Nummererte lister for</span><span class="sxs-lookup"><span data-stu-id="24a0c-116">Numbered lists too</span></span>
    1. <span data-ttu-id="24a0c-117">**Fet** og *kursiv* er a-ok</span><span class="sxs-lookup"><span data-stu-id="24a0c-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="24a0c-118">Koblinger må alltid være enten **"koblinger til Web-område" / ekstern** eller **dyp-koblinger til grensesnittelementene**, ikke interne koblinger.</span><span class="sxs-lookup"><span data-stu-id="24a0c-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="24a0c-119">Og dette er virkelig allerede litt for langt.</span><span class="sxs-lookup"><span data-stu-id="24a0c-119">And this is really already a bit too long.</span></span> <span data-ttu-id="24a0c-120">Beste praksis er omtrent 400 tegn---</span><span class="sxs-lookup"><span data-stu-id="24a0c-120">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="24a0c-121">Når innholdet er klar, drar du den til live grenen.</span><span class="sxs-lookup"><span data-stu-id="24a0c-121">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="24a0c-122">Deretter kan du gå til [partnerportalen på Alkymi](https://alchemyportal.azurewebsites.net) og skriver inn filnavnet i feltet URL-adresse.</span><span class="sxs-lookup"><span data-stu-id="24a0c-122">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="24a0c-123">Kontroller at innsikt gjennomgått og publisert sier "Ja", og klikk deretter Oppdateringsregelen.</span><span class="sxs-lookup"><span data-stu-id="24a0c-123">Make sure Insight reviewed and published says "yes" and then click Update Rule.</span></span> <span data-ttu-id="24a0c-124">**(Dette ser prettier i den nye versjonen av portalen - slippe snart.)** 
 ![URL-adresse-feltet](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="24a0c-124">**(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

