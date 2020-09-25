---
title: eksport verktøy for eDiscovery
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277940"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="1db38-102">Kan du ikke installere eller kjøre eksport verktøyet for eDiscovery?</span><span class="sxs-lookup"><span data-stu-id="1db38-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="1db38-103">Hvis du ikke kan installere eller kjøre eksport verktøyet for eDiscovery for å laste ned søke resultater, kontrollerer du følgende:</span><span class="sxs-lookup"><span data-stu-id="1db38-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="1db38-104">Data maskinen du bruker, oppfyller disse forhånds kravene:</span><span class="sxs-lookup"><span data-stu-id="1db38-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="1db38-105">32-eller 64-biters versjoner av Windows 7 og nyere versjoner</span><span class="sxs-lookup"><span data-stu-id="1db38-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="1db38-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="1db38-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="1db38-107">En støttet nett leser:</span><span class="sxs-lookup"><span data-stu-id="1db38-107">A supported browser:</span></span>

  - <span data-ttu-id="1db38-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="1db38-108">Microsoft Edge</span></span>

    <span data-ttu-id="1db38-109">eller</span><span class="sxs-lookup"><span data-stu-id="1db38-109">Or</span></span>

  - <span data-ttu-id="1db38-110">Internet Explorer 10 og nyere versjoner</span><span class="sxs-lookup"><span data-stu-id="1db38-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="1db38-111">Andre nett lesere, for eksempel Google Chrome og Mozilla Firefox, støttes ikke.</span><span class="sxs-lookup"><span data-stu-id="1db38-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="1db38-112">Organisasjonen kan koble til ende punktet i Azure, som er \*\* \* . blob.Core.Windows.net\*\* (Joker tegnet representerer en unik identifikator for eksport jobben).</span><span class="sxs-lookup"><span data-stu-id="1db38-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="1db38-113">Du er tilordnet eksport rollen i sikkerhets &amp; samsvars senteret for Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1db38-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="1db38-114">Som standard tilordnes denne rollen bare til rolle gruppen for eDiscovery-ansvarlige.</span><span class="sxs-lookup"><span data-stu-id="1db38-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="1db38-115">Se [Tilordne eDiscovery-tillatelser](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="1db38-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="1db38-116">Hvis du vil ha mer informasjon, kan du se [eksportere søke resultater for innhold](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="1db38-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="1db38-117">Hvis du eksporterer mer enn 100K post bokser, må du bruke følgende PowerShell til å laste ned eksport resultatene:  [eksportere resultater fra mer enn 100K post bokser](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="1db38-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>