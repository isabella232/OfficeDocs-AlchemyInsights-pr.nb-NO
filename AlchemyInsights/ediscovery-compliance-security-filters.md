---
title: Ingen resultater ble returnert under innholds søk/eksport
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680334"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="4606f-102">Ingen resultater ble returnert under innholds søk/eksport</span><span class="sxs-lookup"><span data-stu-id="4606f-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="4606f-103">Hvis du har problemer med følgende eDiscovery-scenarioer:</span><span class="sxs-lookup"><span data-stu-id="4606f-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="4606f-104">Innholds søk/eksport returnerer ingen data eller uventede data</span><span class="sxs-lookup"><span data-stu-id="4606f-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="4606f-105">eDiscovery-søk eller eksport mislyktes</span><span class="sxs-lookup"><span data-stu-id="4606f-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="4606f-106">Dette kan være forårsaket av bestemte sikkerhets filtre for samsvar som ble konfigurert av en bestemt administrator, og som ikke er formidlet til alle administratorer.</span><span class="sxs-lookup"><span data-stu-id="4606f-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="4606f-107">Du kan løse dette ved å kontrollere om det finnes noen Samsvars sikkerhets filtre som for år saker disse problemene:</span><span class="sxs-lookup"><span data-stu-id="4606f-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="4606f-108">Koble til sikkerhets-og Samsvars senteret PowerShell</span><span class="sxs-lookup"><span data-stu-id="4606f-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="4606f-109">Kjør følgende cmdleter:</span><span class="sxs-lookup"><span data-stu-id="4606f-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="4606f-110">Hvis du vil ha mer informasjon om Samsvars sikkerhets filtre, kan du se [tillatelses filtrering for innholds søk](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="4606f-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
