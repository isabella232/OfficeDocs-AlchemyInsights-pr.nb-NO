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
# <a name="turn-on-ndi-technology"></a>Aktivere NDI-teknologi

NDI-teknologi krever at to trinn er slått på for en bruker:

1. Leieradministratoren må aktivere egenskapen AllowNDIStreaming i CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Når denne endringen er fylt ut, må sluttbrukeren aktivere NDI®teknologi for den spesifikke klienten fra **Innstillinger > Tillatelser.**

Hvis du vil ha mer informasjon, [kan du se Bruke NDI-teknologi i Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
