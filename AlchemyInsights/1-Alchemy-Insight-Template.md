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
ms.openlocfilehash: 01d8b03209e734f1218de61d964524b1b9e1d044
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939309"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="68b31-102">Nødvendig Alkymi hodet H1, H2's virker ikke.</span><span class="sxs-lookup"><span data-stu-id="68b31-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="68b31-103">Gode fremgangsmåter og retningslinjer for redigering av Alkymi:</span><span class="sxs-lookup"><span data-stu-id="68b31-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="68b31-p101">**Ikke nest Alkymi innsikt i mapper**- dette vil bryte URL-strukturen. Vi er ute til å fikse dette.</span><span class="sxs-lookup"><span data-stu-id="68b31-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="68b31-106">Filene i mappen **AlchemyInsights** skal ha regel-ID og navn på regel fra [Alkymi partnerportal](https://alchemyportal.azurewebsites.net) i filnavnet.</span><span class="sxs-lookup"><span data-stu-id="68b31-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="68b31-p102">f.eks. ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="68b31-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="68b31-p103">Bruke metadata på toppen av denne filen som malen. Ikke noe annet er nødvendig.</span><span class="sxs-lookup"><span data-stu-id="68b31-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="68b31-111">Naviger ned til delen i [Alkymi partnerportal](https://alchemyportal.azurewebsites.net) **kunden innsikt tittel:** og bruk som starter en peker for H1 tittelen for innsikt.</span><span class="sxs-lookup"><span data-stu-id="68b31-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="68b31-p104">Alkymi Insights må bare en enkelt H1 øverst eller de brytes i produksjon. H2s gjengis ikke så Bruk **fet** eller andre konvensjoner på separate deler.</span><span class="sxs-lookup"><span data-stu-id="68b31-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="68b31-114">Deretter fyller du ut brødtekst med kladd-materiale i kunden Insights-delen av siden Alkymi regel</span><span class="sxs-lookup"><span data-stu-id="68b31-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="68b31-115">Punktmerkede lister er greit</span><span class="sxs-lookup"><span data-stu-id="68b31-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="68b31-116">Nummererte lister for</span><span class="sxs-lookup"><span data-stu-id="68b31-116">Numbered lists too</span></span>
    1. <span data-ttu-id="68b31-117">**Fet** og *kursiv* er a-ok</span><span class="sxs-lookup"><span data-stu-id="68b31-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="68b31-118">Koblinger må alltid være enten **"koblinger til Web-område" / ekstern** eller **dyp-koblinger til grensesnittelementene**, ikke interne koblinger.</span><span class="sxs-lookup"><span data-stu-id="68b31-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="68b31-p105">Og dette er virkelig allerede litt for langt. Beste praksis er omtrent 400 tegn---</span><span class="sxs-lookup"><span data-stu-id="68b31-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="68b31-p106">Når innholdet er klar, drar du den til live grenen. Deretter kan du gå til [partnerportalen på Alkymi](https://alchemyportal.azurewebsites.net) og skriver inn filnavnet i feltet URL-adresse. Kontroller at innsikt gjennomgått og publisert sier "Ja", og klikk deretter Oppdateringsregelen. **(Dette ser prettier i den nye versjonen av portalen - slippe snart.)** 
 ![URL-adresse-feltet](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="68b31-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

