---
title: Aktivere NDI-teknologi
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
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935133"
---
# <a name="turn-on-ndi-technology"></a><span data-ttu-id="eda4d-102">Aktivere NDI-teknologi</span><span class="sxs-lookup"><span data-stu-id="eda4d-102">Turn on NDI technology</span></span>

<span data-ttu-id="eda4d-103">NDI-teknologi krever at to trinn er slått på for en bruker:</span><span class="sxs-lookup"><span data-stu-id="eda4d-103">NDI technology requires two steps to be turned on for a user:</span></span>

1. <span data-ttu-id="eda4d-104">Leieradministratoren må aktivere egenskapen AllowNDIStreaming i CsTeamsMeetingPolicy.</span><span class="sxs-lookup"><span data-stu-id="eda4d-104">The tenant admin must enable the 'AllowNDIStreaming' property in CsTeamsMeetingPolicy.</span></span>

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. <span data-ttu-id="eda4d-105">Når denne endringen er fylt ut, må sluttbrukeren aktivere NDI®teknologi for den spesifikke klienten fra **Innstillinger > Tillatelser.**</span><span class="sxs-lookup"><span data-stu-id="eda4d-105">After this change has populated, the end user must turn on NDI® technology for their specific client from **Settings > Permissions**.</span></span>

<span data-ttu-id="eda4d-106">Hvis du vil ha mer informasjon, [kan du se Bruke NDI-teknologi i Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)</span><span class="sxs-lookup"><span data-stu-id="eda4d-106">For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span></span>
