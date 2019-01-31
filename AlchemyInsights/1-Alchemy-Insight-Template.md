---
title: 'samme som filnavnet er best [REGEL #-beskrivelse]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 1bb1cb35f06e16a2dc85b7e2642b9fa0d203945e
ms.sourcegitcommit: b032c2ac45540b1eb5dd68a4ec7ce1a5d6922f0e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662939"
---
# <a name="required-customer-facing-h1-h2-doesnt-work"></a><span data-ttu-id="2dd2a-102">Nødvendige kunden motstående H1, H2 fungerer ikke</span><span class="sxs-lookup"><span data-stu-id="2dd2a-102">Required Customer Facing H1, H2 doesn't work</span></span>
<span data-ttu-id="2dd2a-103">Eksempeltekst blokker - Følg disse instruksjonene:</span><span class="sxs-lookup"><span data-stu-id="2dd2a-103">Example text block - follow these instructions:</span></span>

1. <span data-ttu-id="2dd2a-104">Filene i mappen **AlchemyInsights** skal ha regel-ID og navn på regel fra [Alkymi partnerportal](https://alchemyportal.azurewebsites.net) i filnavnet.</span><span class="sxs-lookup"><span data-stu-id="2dd2a-104">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="2dd2a-p101">f.eks. ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="2dd2a-p101">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="2dd2a-p102">Bruke metadata på toppen av denne filen som malen. Ikke noe annet er nødvendig.</span><span class="sxs-lookup"><span data-stu-id="2dd2a-p102">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="2dd2a-109">Naviger ned til delen i [Alkymi partnerportal](https://alchemyportal.azurewebsites.net) **kunden innsikt tittel:** og bruk som starter en peker for H1 tittelen for innsikt.</span><span class="sxs-lookup"><span data-stu-id="2dd2a-109">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="2dd2a-p103">Alkymi Insights må bare en enkelt H1 øverst eller de brytes i produksjon. H2s gjengis ikke så Bruk **fet** eller andre konvensjoner på separate deler.</span><span class="sxs-lookup"><span data-stu-id="2dd2a-p103">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="2dd2a-112">Deretter fyller du ut brødtekst med kladd-materiale i kunden Insights-delen av siden Alkymi regel</span><span class="sxs-lookup"><span data-stu-id="2dd2a-112">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="2dd2a-113">Punktmerkede lister er greit</span><span class="sxs-lookup"><span data-stu-id="2dd2a-113">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="2dd2a-114">Nummererte lister for</span><span class="sxs-lookup"><span data-stu-id="2dd2a-114">Numbered lists too</span></span>
    1. <span data-ttu-id="2dd2a-115">**Fet** og *kursiv* er a-ok</span><span class="sxs-lookup"><span data-stu-id="2dd2a-115">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="2dd2a-116">Koblinger må alltid være enten **"koblinger til Web-område" / ekstern** eller **dyp-koblinger til grensesnittelementene**, ikke interne koblinger.</span><span class="sxs-lookup"><span data-stu-id="2dd2a-116">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="2dd2a-p104">Og dette er virkelig allerede litt for langt. Beste praksis er omtrent 400 tegn---</span><span class="sxs-lookup"><span data-stu-id="2dd2a-p104">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="2dd2a-p105">Når innholdet er klar, drar du den til live grenen. Deretter kan du gå til [partnerportalen på Alkymi](https://alchemyportal.azurewebsites.net) og skriver inn filnavnet i feltet URL-adresse. Kontroller at innsikt gjennomgått og publisert sier "Ja", og klikk deretter Oppdateringsregelen. (Dette ser prettier i den nye versjonen av portalen - slippe snart.)</span><span class="sxs-lookup"><span data-stu-id="2dd2a-p105">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. (This will look prettier in the new version of the portal - releasing soon.)</span></span>

![URL-adresse-feltet](media/for-content-team.PNG)

