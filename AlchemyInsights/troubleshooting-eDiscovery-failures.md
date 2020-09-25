---
title: 1490 – feil søking – eDiscovery-feil
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277812"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="2e34a-102">Feilsøke innholds søke feil</span><span class="sxs-lookup"><span data-stu-id="2e34a-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="2e34a-103">Har du problemer med innholds søk, eller får feil når du eksporterer søke resultater?</span><span class="sxs-lookup"><span data-stu-id="2e34a-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="2e34a-104">Vil du for eksempel motta følgende når du kjører søk?</span><span class="sxs-lookup"><span data-stu-id="2e34a-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="2e34a-105">CS008-eller CS012-feil</span><span class="sxs-lookup"><span data-stu-id="2e34a-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="2e34a-106">Feil med opptatt/tids avbrudd for server</span><span class="sxs-lookup"><span data-stu-id="2e34a-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="2e34a-107">Program feil oppstod</span><span class="sxs-lookup"><span data-stu-id="2e34a-107">Application error occurred</span></span>

<span data-ttu-id="2e34a-108">Eller når du søker etter eller eksporterer resultater fra et stort antall post bokser (over 100 000 post bokser), får du eksport feil?</span><span class="sxs-lookup"><span data-stu-id="2e34a-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="2e34a-109">For disse feil typene kan du prøve Søk på nytt for innholds plasseringer som har mislyktes.</span><span class="sxs-lookup"><span data-stu-id="2e34a-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="2e34a-110">Se  [denne artikkelen](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) hvis du vil ha mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="2e34a-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="2e34a-111">Hvis du eksporterer mer enn 100K post bokser, må du bruke følgende PowerShell til å laste ned eksport resultatene:  [eksportere resultater fra mer enn 100K post bokser](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="2e34a-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
