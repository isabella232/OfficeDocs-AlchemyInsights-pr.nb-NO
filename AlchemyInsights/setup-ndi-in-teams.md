---
title: Slå på NDI-teknologi
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
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023531"
---
# <a name="turn-on-ndi-technology"></a>Slå på NDI-teknologi

NDI-teknologi krever at to trinn er aktivert for en bruker:

1. Leieradministratoren må aktivere egenskapen AllowNDIStreaming i CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Når denne endringen er fylt ut, må sluttbrukeren aktivere NDI®-teknologi for den bestemte klienten fra **Innstillinger > Tillatelser**.

Hvis du vil ha mer informasjon, kan du se Bruke [NDI-teknologi i Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
