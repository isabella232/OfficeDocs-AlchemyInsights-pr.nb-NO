---
title: samme som filnavn er best
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676542"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="3d6e7-102">Krevde Alchemy Header H1, H2's fungerer ikke.</span><span class="sxs-lookup"><span data-stu-id="3d6e7-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="3d6e7-103">Beste praksis og retningslinjer for Alkymi redigering:</span><span class="sxs-lookup"><span data-stu-id="3d6e7-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="3d6e7-104">**Ikke neste Alchemy Insights i mapper**- dette vil bryte url strukturen.</span><span class="sxs-lookup"><span data-stu-id="3d6e7-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="3d6e7-105">Vi undersøker dette.</span><span class="sxs-lookup"><span data-stu-id="3d6e7-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="3d6e7-106">Filer i **AlchemyInsights-mappen** bør ha små filnavn med bindestreker for mellomrom ex.</span><span class="sxs-lookup"><span data-stu-id="3d6e7-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="3d6e7-107">***hvordan-å-aktivere-rettstvist-hold***.</span><span class="sxs-lookup"><span data-stu-id="3d6e7-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="3d6e7-108">Inkluder regel-ID-en eller samlings-IDen fra [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net) i ms.custom-feltet.</span><span class="sxs-lookup"><span data-stu-id="3d6e7-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="3d6e7-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="3d6e7-109">ex.</span></span> <span data-ttu-id="3d6e7-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="3d6e7-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="3d6e7-111">Bruk resten av metadataene øverst i denne filen som mal.</span><span class="sxs-lookup"><span data-stu-id="3d6e7-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="3d6e7-112">I [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net)navigerer du ned til delen **Customer Insight-tittel:** og bruk dette som utgangspunkt for H1-tittelen for innsikten.</span><span class="sxs-lookup"><span data-stu-id="3d6e7-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="3d6e7-113">Alchemy Insights MÅ bare ha en enkelt H1 på toppen, ellerde vil bryte i produksjon.</span><span class="sxs-lookup"><span data-stu-id="3d6e7-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="3d6e7-114">H2s ikke gjengi enten så bruk **fet eller** andre konvensjoner for å betegne separate seksjoner.</span><span class="sxs-lookup"><span data-stu-id="3d6e7-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="3d6e7-115">Deretter fyller du ut brødteksten ved hjelp av utkastet til materiale i Kundeinnsikt-delen på Siden Alchemy-regel</span><span class="sxs-lookup"><span data-stu-id="3d6e7-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="3d6e7-116">Punktlister er fine</span><span class="sxs-lookup"><span data-stu-id="3d6e7-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="3d6e7-117">Nummererte lister også</span><span class="sxs-lookup"><span data-stu-id="3d6e7-117">Numbered lists too</span></span>
    1. <span data-ttu-id="3d6e7-118">**Fet** og *kursiv* er a-ok</span><span class="sxs-lookup"><span data-stu-id="3d6e7-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="3d6e7-119">Lenker bør alltid være enten **"lenker til web"/eksterne** ELLER **dyplenker til brukerelementer**, ikke interne lenker.</span><span class="sxs-lookup"><span data-stu-id="3d6e7-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="3d6e7-120">Bilder støttes ikke offisielt på dette tidspunktet, men det er på veikartet.</span><span class="sxs-lookup"><span data-stu-id="3d6e7-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="3d6e7-121">Og dette er egentlig allerede litt for lenge.</span><span class="sxs-lookup"><span data-stu-id="3d6e7-121">And this is really already a bit too long.</span></span> <span data-ttu-id="3d6e7-122">Beste praksis er ca 400 tegn ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="3d6e7-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="3d6e7-123">Når innholdet er klart, trekker du det til den direktesendte grenen.</span><span class="sxs-lookup"><span data-stu-id="3d6e7-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="3d6e7-124">Deretter går du til [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net) og skriver inn filnavnet i url-feltet.</span><span class="sxs-lookup"><span data-stu-id="3d6e7-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 