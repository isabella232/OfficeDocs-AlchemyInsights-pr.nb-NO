---
title: Innholds søk ingen resultater
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
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680656"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="174c2-102">Ingen resultater fra innholds søk/eksporterer</span><span class="sxs-lookup"><span data-stu-id="174c2-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="174c2-103">Problemer med innholds søk/Eksporter som ikke returnerer data, kan være på grunn av bestemte sikkerhets filtre for samsvar som ble konfigurert av en bestemt administrator, og ikke formidle det til alle administratorer.</span><span class="sxs-lookup"><span data-stu-id="174c2-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="174c2-104">Du kan løse dette ved å kontrollere om det finnes noen Samsvars sikkerhets filtre som gjør dette:</span><span class="sxs-lookup"><span data-stu-id="174c2-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="174c2-105">Koble til sikkerhets-og Samsvars senteret PowerShell</span><span class="sxs-lookup"><span data-stu-id="174c2-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="174c2-106">Kjør følgende cmdleter:</span><span class="sxs-lookup"><span data-stu-id="174c2-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="174c2-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="174c2-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="174c2-108">Get-ComplianceSecurityFilter-Organization $org</span><span class="sxs-lookup"><span data-stu-id="174c2-108">Get-ComplianceSecurityFilter -Organization $org</span></span>