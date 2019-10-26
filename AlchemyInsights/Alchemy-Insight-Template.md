---
title: samme som filnavn er best
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/25/2019
ms.locfileid: "35800054"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="70105-102">Krevde alkymi overskriften H1, H2's dont ' arbeide.</span><span class="sxs-lookup"><span data-stu-id="70105-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="70105-103">Best Practices og retningslinjer for Alchemy authoring:</span><span class="sxs-lookup"><span data-stu-id="70105-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="70105-104">**Ikke hekker Alchemy Insights i mapper**-dette vil bryte URL strukturen.</span><span class="sxs-lookup"><span data-stu-id="70105-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="70105-105">Vi ser på å fikse dette.</span><span class="sxs-lookup"><span data-stu-id="70105-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="70105-106">Filer i mappen **AlchemyInsights** bør ha små filnavn med bindestreker for mellomrom.</span><span class="sxs-lookup"><span data-stu-id="70105-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="70105-107">***hvordan-å-aktivere-søksmål-Hold***.</span><span class="sxs-lookup"><span data-stu-id="70105-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="70105-108">Inkluder regel-ID eller Bucket ID fra [Alchemy partner-portalen](https://alchemyportal.azurewebsites.net) i det egendefinerte feltet MS.</span><span class="sxs-lookup"><span data-stu-id="70105-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="70105-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="70105-109">ex.</span></span> <span data-ttu-id="70105-110">***MS Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="70105-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="70105-111">Bruk resten av metadataene øverst i denne filen som mal.</span><span class="sxs-lookup"><span data-stu-id="70105-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="70105-112">I [Alchemy partner Portal](https://alchemyportal.azurewebsites.net), Naviger ned til seksjonen **Customer Insight tittel:** og bruke det som et utgangspunkt for H1 tittel for innsikt.</span><span class="sxs-lookup"><span data-stu-id="70105-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="70105-113">Alchemy Insights må ha bare en enkelt H1 på toppen eller de vil bryte i produksjon.</span><span class="sxs-lookup"><span data-stu-id="70105-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="70105-114">H2s ikke gjengi enten så bruk **fet** eller andre konvensjoner for å betegne separate seksjoner.</span><span class="sxs-lookup"><span data-stu-id="70105-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="70105-115">Deretter fyller du ut brødteksten ved hjelp av kladde materialet i delen Kundeinnsikt på siden alkymi-regel</span><span class="sxs-lookup"><span data-stu-id="70105-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="70105-116">Punktmerkede lister er fine</span><span class="sxs-lookup"><span data-stu-id="70105-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="70105-117">Nummererte lister også</span><span class="sxs-lookup"><span data-stu-id="70105-117">Numbered lists too</span></span>
    1. <span data-ttu-id="70105-118">**Fet** og *kursiv* er en-OK</span><span class="sxs-lookup"><span data-stu-id="70105-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="70105-119">Linker bør alltid være enten **"lenker til Web"/External** eller **Deep-linker til UI elementer**, ikke interne koblinger.</span><span class="sxs-lookup"><span data-stu-id="70105-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="70105-120">Bilder er ikke offisielt støttet på dette tidspunktet, men det er på veikart.</span><span class="sxs-lookup"><span data-stu-id="70105-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="70105-121">Og dette er egentlig allerede litt for lang.</span><span class="sxs-lookup"><span data-stu-id="70105-121">And this is really already a bit too long.</span></span> <span data-ttu-id="70105-122">Beste praksis er om 400 tegn---------------------------------</span><span class="sxs-lookup"><span data-stu-id="70105-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="70105-123">Når innholdet er klart, drar du det til den aktive grenen.</span><span class="sxs-lookup"><span data-stu-id="70105-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="70105-124">Deretter går du til [alkymi partner portalen](https://alchemyportal.azurewebsites.net) og skriv inn filnavnet i URL-feltet.</span><span class="sxs-lookup"><span data-stu-id="70105-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 