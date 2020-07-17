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
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750979"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="5c5a4-102">"Krevde Alkymi Header H1, H2's fungerer ikke."</span><span class="sxs-lookup"><span data-stu-id="5c5a4-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="5c5a4-103">Beste praksis og retningslinjer for alkymiredigering:</span><span class="sxs-lookup"><span data-stu-id="5c5a4-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="5c5a4-104">**Ikke nest Alchemy Insights i mapper**- dette vil bryte url-strukturen.</span><span class="sxs-lookup"><span data-stu-id="5c5a4-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="5c5a4-105">Vi undersøker dette.</span><span class="sxs-lookup"><span data-stu-id="5c5a4-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="5c5a4-106">Filer i **AlchemyInsights-mappen** bør ha små bokstaver med bindestreker for mellomrom ex.</span><span class="sxs-lookup"><span data-stu-id="5c5a4-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="5c5a4-107">***how-to-enable-litigation-hold***.</span><span class="sxs-lookup"><span data-stu-id="5c5a4-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="5c5a4-108">Inkluder regel-ID-en eller bucket-ID-en fra [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net) i ms.custom-feltet.</span><span class="sxs-lookup"><span data-stu-id="5c5a4-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="5c5a4-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="5c5a4-109">ex.</span></span> <span data-ttu-id="5c5a4-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="5c5a4-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="5c5a4-111">Bruk resten av metadataene øverst i denne filen som mal.</span><span class="sxs-lookup"><span data-stu-id="5c5a4-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="5c5a4-112">I [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net)navigerer du ned til delen **Customer Insight-tittel,** og bruker det som utgangspunkt for H1-tittelen for innsikten.</span><span class="sxs-lookup"><span data-stu-id="5c5a4-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="5c5a4-113">Alchemy Insights MÅ ha bare en enkelt H1 på toppen, eller de vil bryte i produksjon.</span><span class="sxs-lookup"><span data-stu-id="5c5a4-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="5c5a4-114">H2s gjengis ikke, så bruk **fet eller** andre konvensjoner for å betegne separate deler.</span><span class="sxs-lookup"><span data-stu-id="5c5a4-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="5c5a4-115">Deretter fyller du ut brødteksten ved hjelp av kladdematerialet i Kundeinnsikt-delen på Alchemy Rule-siden</span><span class="sxs-lookup"><span data-stu-id="5c5a4-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="5c5a4-116">Punktlister er fine</span><span class="sxs-lookup"><span data-stu-id="5c5a4-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="5c5a4-117">Nummererte lister også</span><span class="sxs-lookup"><span data-stu-id="5c5a4-117">Numbered lists too</span></span>
    1. <span data-ttu-id="5c5a4-118">**Fet** og *kursiv* er a-ok</span><span class="sxs-lookup"><span data-stu-id="5c5a4-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="5c5a4-119">Lenker bør alltid være **enten "lenker til web"/eksterne** ELLER **dypkoblinger til UI-elementer**, ikke interne koblinger.</span><span class="sxs-lookup"><span data-stu-id="5c5a4-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="5c5a4-120">Bilder støttes ikke offisielt på dette tidspunktet, men det er på veikartet.</span><span class="sxs-lookup"><span data-stu-id="5c5a4-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="5c5a4-121">Og dette er egentlig allerede litt for lenge.</span><span class="sxs-lookup"><span data-stu-id="5c5a4-121">And this is really already a bit too long.</span></span> <span data-ttu-id="5c5a4-122">Beste praksis er ca 400 tegn ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="5c5a4-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="5c5a4-123">Når innholdet er klart, trekker du det til den aktive grenen.</span><span class="sxs-lookup"><span data-stu-id="5c5a4-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="5c5a4-124">Deretter går du til [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net) og skriver inn filnavnet i url-feltet.</span><span class="sxs-lookup"><span data-stu-id="5c5a4-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 