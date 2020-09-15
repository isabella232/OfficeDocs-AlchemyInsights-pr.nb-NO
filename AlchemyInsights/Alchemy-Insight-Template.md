---
title: samme som fil navnet er best
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664143"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="432ee-102">"Obligatorisk Alchemy-hode H1, H2's fungerer ikke."</span><span class="sxs-lookup"><span data-stu-id="432ee-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="432ee-103">Beste Fremgangs måter og retnings linjer for Alchemy redigering:</span><span class="sxs-lookup"><span data-stu-id="432ee-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="432ee-104">Ikke **neste Alchemye innsikt i mapper**– dette vil bryte URL-strukturen.</span><span class="sxs-lookup"><span data-stu-id="432ee-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="432ee-105">Vi er i ferd med å rette opp dette.</span><span class="sxs-lookup"><span data-stu-id="432ee-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="432ee-106">Filer i **AlchemyInsights** -mappen bør ha små bokstaver med binde streker for mellomrom ex.</span><span class="sxs-lookup"><span data-stu-id="432ee-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="432ee-107">Fremgangs ***måte for aktivering – retts tvist-vent***.</span><span class="sxs-lookup"><span data-stu-id="432ee-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="432ee-108">Inkluder regel-ID-en eller spann-ID-en fra [Alchemy partner Portal](https://alchemyportal.azurewebsites.net) i MS. Custom-feltet.</span><span class="sxs-lookup"><span data-stu-id="432ee-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="432ee-109">&.</span><span class="sxs-lookup"><span data-stu-id="432ee-109">ex.</span></span> <span data-ttu-id="432ee-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="432ee-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="432ee-111">Bruk resten av metadataene øverst i denne filen som mal.</span><span class="sxs-lookup"><span data-stu-id="432ee-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="432ee-112">I [Alchemy partner portalen](https://alchemyportal.azurewebsites.net)navigerer du ned til inndelingen **kunde innsikt tittel:** og bruker dette som et utgangs punkt for den H1-tittelen for innsiktet.</span><span class="sxs-lookup"><span data-stu-id="432ee-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="432ee-113">Alchemy innsikter må ha bare én enkelt H1 øverst, eller de kommer til å bryte i produksjon.</span><span class="sxs-lookup"><span data-stu-id="432ee-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="432ee-114">H2s ikke gjengir, så du kan bruke **fet** eller andre konvensjoner til å skille mellom separate inndelinger.</span><span class="sxs-lookup"><span data-stu-id="432ee-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="432ee-115">Deretter fyller du ut brød teksten ved hjelp av kladde materialet i delen kunde innsikt på Alchemy Regels IDen</span><span class="sxs-lookup"><span data-stu-id="432ee-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="432ee-116">Punkt lister er fine</span><span class="sxs-lookup"><span data-stu-id="432ee-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="432ee-117">Nummererte lister</span><span class="sxs-lookup"><span data-stu-id="432ee-117">Numbered lists too</span></span>
    1. <span data-ttu-id="432ee-118">**Fet** og *kursiv* er en-OK</span><span class="sxs-lookup"><span data-stu-id="432ee-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="432ee-119">Koblinger må alltid være enten **koblinger til Web-/External** eller **dype koblinger til grensesnitt elementer**, ikke interne koblinger.</span><span class="sxs-lookup"><span data-stu-id="432ee-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="432ee-120">Bilder støttes ikke offisielt på dette tidspunktet, men det er på vei kartet.</span><span class="sxs-lookup"><span data-stu-id="432ee-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="432ee-121">Og dette er faktisk allerede litt for langt.</span><span class="sxs-lookup"><span data-stu-id="432ee-121">And this is really already a bit too long.</span></span> <span data-ttu-id="432ee-122">Beste Fremgangs måte er omtrent 400 tegn---------------------------------</span><span class="sxs-lookup"><span data-stu-id="432ee-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="432ee-123">Når innholdet er klart, kan du dra det til direkte grenen.</span><span class="sxs-lookup"><span data-stu-id="432ee-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="432ee-124">Gå deretter til [Alchemy partner Portal](https://alchemyportal.azurewebsites.net) , og skriv inn fil navnet i URL-feltet.</span><span class="sxs-lookup"><span data-stu-id="432ee-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 