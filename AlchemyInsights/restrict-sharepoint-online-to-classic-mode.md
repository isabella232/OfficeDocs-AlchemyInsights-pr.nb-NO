---
title: Begrense SharePoint Online til klassisk modus
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 52c63d8909796f8d0d114a46c5255e4073e8c47d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35369782"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="8eeed-102">Begrense SharePoint Online til klassisk modus</span><span class="sxs-lookup"><span data-stu-id="8eeed-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="8eeed-103">Noen organisasjoner krever fortsatt klassisk modus-opplevelse.</span><span class="sxs-lookup"><span data-stu-id="8eeed-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="8eeed-104">Mens det er ingen planer om å fjerne klassisk modus på et detaljert nivå, er det ikke lenger mulig å begrense en hel organisasjon (leier) til klassisk modus for lister og biblioteker.</span><span class="sxs-lookup"><span data-stu-id="8eeed-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="8eeed-105">Administratoren har følgende alternativer for å administrere individuelle lister og biblioteker i klassisk modus ved hjelp av detaljerte opt-out-brytere som vi gir på følgende nivåer:</span><span class="sxs-lookup"><span data-stu-id="8eeed-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="8eeed-106">områdesamling</span><span class="sxs-lookup"><span data-stu-id="8eeed-106">site collection</span></span>
- <span data-ttu-id="8eeed-107">området</span><span class="sxs-lookup"><span data-stu-id="8eeed-107">site</span></span>
- <span data-ttu-id="8eeed-108">liste</span><span class="sxs-lookup"><span data-stu-id="8eeed-108">list</span></span>
- <span data-ttu-id="8eeed-109">biblioteket</span><span class="sxs-lookup"><span data-stu-id="8eeed-109">library</span></span>

<span data-ttu-id="8eeed-110">I tillegg vil lister som bruker bestemte funksjoner og tilpasninger som ikke støttes av moderne fortsatt være automatisk byttet til klassisk modus.</span><span class="sxs-lookup"><span data-stu-id="8eeed-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="8eeed-111">Fra April 1, 2019, prosessen for å deaktivere leier nivået unnlate moderne liste og biblioteker starter, og fortsetter gjennom den 31 mai 2019.</span><span class="sxs-lookup"><span data-stu-id="8eeed-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="8eeed-112">Listene og bibliotekene som er i klassisk modus som et resultat av leier deltatt vil automatisk bli forskjøvet til moderne.</span><span class="sxs-lookup"><span data-stu-id="8eeed-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="8eeed-113">Hvis du trenger klassisk modus kan du se mer informasjon [her](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) og PnP Powershell instruksjon [her](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) som beskriver alternativer og verktøy du kan bruke i dag å Bruk Klassisk modus-opplevelse.</span><span class="sxs-lookup"><span data-stu-id="8eeed-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
