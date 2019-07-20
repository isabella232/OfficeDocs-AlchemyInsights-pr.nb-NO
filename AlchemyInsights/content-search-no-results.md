---
title: Ingen resultat av søk innhold
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800490"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="b7d5e-102">Ingen resultater fra innhold Søk/Eksporter</span><span class="sxs-lookup"><span data-stu-id="b7d5e-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="b7d5e-103">Problemer med innhold Søk/eksporterer ikke returnerte noen data kan være på grunn av visse overholdelse sikkerhetsfilter som var installasjonen av et bestemt Admin og kommuniserer ikke til alle administratorer.</span><span class="sxs-lookup"><span data-stu-id="b7d5e-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="b7d5e-104">Hvis du vil løse dette problemet, kontrollerer du om det er samsvar sikkerhetsfiltre som kan forårsake dette:</span><span class="sxs-lookup"><span data-stu-id="b7d5e-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="b7d5e-105">Koble til sikkerhet og overholdelse Center Powershell</span><span class="sxs-lookup"><span data-stu-id="b7d5e-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="b7d5e-106">Kjør følgende kommandleter:</span><span class="sxs-lookup"><span data-stu-id="b7d5e-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="b7d5e-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="b7d5e-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="b7d5e-108">Get-ComplianceSecurityFilter-$org for organisasjon</span><span class="sxs-lookup"><span data-stu-id="b7d5e-108">Get-ComplianceSecurityFilter -Organization $org</span></span>