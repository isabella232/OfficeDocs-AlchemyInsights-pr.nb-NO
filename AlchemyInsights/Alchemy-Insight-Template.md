---
title: samme som filnavnet er best
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 5555
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 68f743ee9c448565470815f8410cc6ce4b384bed
ms.sourcegitcommit: 0b6e9470c6b73616ba8bacef7010f739b7fac332
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/21/2019
ms.locfileid: "30742434"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="4f217-102">Nødvendig Alkymi hodet H1, H2's virker ikke.</span><span class="sxs-lookup"><span data-stu-id="4f217-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="4f217-103">Gode fremgangsmåter og retningslinjer for redigering av Alkymi:</span><span class="sxs-lookup"><span data-stu-id="4f217-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="4f217-104">**Ikke nest Alkymi innsikt i mapper**- dette vil bryte URL-strukturen.</span><span class="sxs-lookup"><span data-stu-id="4f217-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="4f217-105">Vi er ute til å fikse dette.</span><span class="sxs-lookup"><span data-stu-id="4f217-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="4f217-106">Filene i mappen **AlchemyInsights** skal ha små bokstaver filnavn med bindestreker for mellomrom ex.</span><span class="sxs-lookup"><span data-stu-id="4f217-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="4f217-107">***how-skal aktivere-rettstvist-Vent***.</span><span class="sxs-lookup"><span data-stu-id="4f217-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="4f217-108">Ta med regel-ID eller bucket ID fra [Alkymi partnerportal](https://alchemyportal.azurewebsites.net) i feltet ms.custom.</span><span class="sxs-lookup"><span data-stu-id="4f217-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="4f217-109">EX.</span><span class="sxs-lookup"><span data-stu-id="4f217-109">ex.</span></span> <span data-ttu-id="4f217-110">***MS.Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="4f217-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="4f217-111">Bruk resten av metadataene på toppen av denne filen som malen.</span><span class="sxs-lookup"><span data-stu-id="4f217-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="4f217-112">Naviger ned til delen i [Alkymi partnerportal](https://alchemyportal.azurewebsites.net) **kunden innsikt tittel:** og bruk som starter en peker for H1 tittelen for innsikt.</span><span class="sxs-lookup"><span data-stu-id="4f217-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="4f217-113">Alkymi Insights må bare en enkelt H1 øverst eller de brytes i produksjon.</span><span class="sxs-lookup"><span data-stu-id="4f217-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="4f217-114">H2s gjengis ikke så Bruk **fet** eller andre konvensjoner på separate deler.</span><span class="sxs-lookup"><span data-stu-id="4f217-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="4f217-115">Deretter fyller du ut brødtekst med kladd-materiale i kunden Insights-delen av siden Alkymi regel</span><span class="sxs-lookup"><span data-stu-id="4f217-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="4f217-116">Punktmerkede lister er greit</span><span class="sxs-lookup"><span data-stu-id="4f217-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="4f217-117">Nummererte lister for</span><span class="sxs-lookup"><span data-stu-id="4f217-117">Numbered lists too</span></span>
    1. <span data-ttu-id="4f217-118">**Fet** og *kursiv* er a-ok</span><span class="sxs-lookup"><span data-stu-id="4f217-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="4f217-119">Koblinger må alltid være enten **"koblinger til Web-område" / ekstern** eller **dyp-koblinger til grensesnittelementene**, ikke interne koblinger.</span><span class="sxs-lookup"><span data-stu-id="4f217-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="4f217-120">Bilder offisielt støtter ikke denne gangen, men det er på veikartet for tiltaket.</span><span class="sxs-lookup"><span data-stu-id="4f217-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="4f217-121">Og dette er virkelig allerede litt for langt.</span><span class="sxs-lookup"><span data-stu-id="4f217-121">And this is really already a bit too long.</span></span> <span data-ttu-id="4f217-122">Beste praksis er omtrent 400 tegn---</span><span class="sxs-lookup"><span data-stu-id="4f217-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="4f217-123">Når innholdet er klar, drar du den til live grenen.</span><span class="sxs-lookup"><span data-stu-id="4f217-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="4f217-124">Deretter kan du gå til [partnerportalen på Alkymi](https://alchemyportal.azurewebsites.net) og skriver inn filnavnet i feltet URL-adresse.</span><span class="sxs-lookup"><span data-stu-id="4f217-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="4f217-125">M</span><span class="sxs-lookup"><span data-stu-id="4f217-125">M</span></span>