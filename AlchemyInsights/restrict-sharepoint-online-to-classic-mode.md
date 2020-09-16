---
title: Begrense SharePoint Online til klassisk modus
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751431"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="29beb-102">Begrense SharePoint Online til klassisk modus</span><span class="sxs-lookup"><span data-stu-id="29beb-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="29beb-103">Enkelte organisasjoner trenger fremdeles den klassiske modus opplevelsen.</span><span class="sxs-lookup"><span data-stu-id="29beb-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="29beb-104">Selv om det ikke er noen planer om å fjerne klassisk modus på et detaljert nivå, er det ikke lenger mulig å begrense en hel organisasjon (Tenant) til klassisk modus for lister og biblioteker.</span><span class="sxs-lookup"><span data-stu-id="29beb-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="29beb-105">Administratoren vil ha følgende alternativer for å administrere individuelle lister og biblioteker i klassisk modus ved hjelp av detaljerte utvalgs brytere som vi tilbyr på følgende nivåer:</span><span class="sxs-lookup"><span data-stu-id="29beb-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="29beb-106">område samling</span><span class="sxs-lookup"><span data-stu-id="29beb-106">site collection</span></span>
- <span data-ttu-id="29beb-107">Web</span><span class="sxs-lookup"><span data-stu-id="29beb-107">site</span></span>
- <span data-ttu-id="29beb-108">tilgangskontrolliste</span><span class="sxs-lookup"><span data-stu-id="29beb-108">list</span></span>
- <span data-ttu-id="29beb-109">biblioteket</span><span class="sxs-lookup"><span data-stu-id="29beb-109">library</span></span>

<span data-ttu-id="29beb-110">I tillegg vil lister som bruker bestemte funksjoner og tilpasninger som ikke støttes av moderne, automatisk byttes til klassisk modus.</span><span class="sxs-lookup"><span data-stu-id="29beb-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="29beb-111">Begynnelsen 1. april 2019, og prosessen for å deaktivere leie nivået for å velge ut av moderne liste og biblioteker, starter og fortsetter til og med 31, 2019.</span><span class="sxs-lookup"><span data-stu-id="29beb-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="29beb-112">Listene og bibliotekene i klassisk modus som følge av leier, blir automatisk flyttet til moderne.</span><span class="sxs-lookup"><span data-stu-id="29beb-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="29beb-113">Hvis du trenger klassisk modus, kan du se mer informasjon [her](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) og PnP PowerShell-instruksjon [her](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) som beskriver alternativer og verktøy du kan bruke i dag, til å bruke den klassiske modus opplevelsen.</span><span class="sxs-lookup"><span data-stu-id="29beb-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
