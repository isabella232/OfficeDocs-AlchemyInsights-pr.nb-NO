---
title: Eksportverktøy for eDiscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814597"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="b5b67-102">Kan du ikke installere eller kjøre eksportverktøyet for eDiscovery?</span><span class="sxs-lookup"><span data-stu-id="b5b67-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="b5b67-103">Hvis du ikke kan installere eller kjøre eksportverktøyet for eDiscovery for å laste ned søkeresultater, kontrollerer du følgende:</span><span class="sxs-lookup"><span data-stu-id="b5b67-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="b5b67-104">Datamaskinen du bruker, oppfyller disse forhåndskravene:</span><span class="sxs-lookup"><span data-stu-id="b5b67-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="b5b67-105">32- eller 64-biters versjoner av Windows 7 og nyere versjoner</span><span class="sxs-lookup"><span data-stu-id="b5b67-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="b5b67-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="b5b67-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="b5b67-107">En støttet nettleser:</span><span class="sxs-lookup"><span data-stu-id="b5b67-107">A supported browser:</span></span>

  - <span data-ttu-id="b5b67-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="b5b67-108">Microsoft Edge</span></span>

    <span data-ttu-id="b5b67-109">eller</span><span class="sxs-lookup"><span data-stu-id="b5b67-109">Or</span></span>

  - <span data-ttu-id="b5b67-110">Internet Explorer 10 og nyere versjoner</span><span class="sxs-lookup"><span data-stu-id="b5b67-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="b5b67-111">Andre nettlesere, for eksempel Google Chrome og Mozilla Firefox, støttes ikke.</span><span class="sxs-lookup"><span data-stu-id="b5b67-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="b5b67-112">Organisasjonen kan koble til endepunktet i Azure, som er **\* .blob.core.windows.net** (jokertegnet representerer en unik identifikator for eksportjobben).</span><span class="sxs-lookup"><span data-stu-id="b5b67-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="b5b67-113">Du er tilordnet eksportrollen i sikkerhetssamsvarssenteret for Microsoft 365. &amp;</span><span class="sxs-lookup"><span data-stu-id="b5b67-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="b5b67-114">Denne rollen tilordnes som standard bare til rollegruppen eDiscovery Manager.</span><span class="sxs-lookup"><span data-stu-id="b5b67-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="b5b67-115">Se [Tilordne eDiscovery-tillatelser](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="b5b67-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="b5b67-116">Hvis du vil ha mer informasjon, [kan du se Eksportere søkeresultater for innhold](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="b5b67-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="b5b67-117">Hvis du eksporterer mer enn 100 000 postbokser, må du bruke følgende Powershell til å laste ned eksportresultatene: Eksportere resultater fra mer enn  [100 000 postbokser](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="b5b67-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>