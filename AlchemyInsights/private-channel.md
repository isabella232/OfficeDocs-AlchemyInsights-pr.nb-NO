---
title: Privat kanal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005447"
---
# <a name="private-channels-in-microsoft-teams"></a>Private kanaler i Microsoft Teams

Private kanaler er en ny funksjon i Microsoft Teams. Vær oppmerksom på at private kanaler ikke kan konverteres fra standardkanaler eller omvendt.

Hvis du vil ha mer informasjon om private kanaler, for eksempel informasjon om [oppretting og medlemskap](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) i private kanaler og [SharePoint-områder](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)i private kanaler, kan du se Private kanaler i Microsoft [Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Merk:** Fordi konfigurasjon for oppbevaring av private kanalmeldinger ennå ikke støttes, vil ikke leietakere med oppbevaringspolicyer aktivert ha private kanaler aktivert som standard. Private kanaler kan aktiveres i teams administrasjonssenter. Vær også oppmerksom på at selv om oppbevaring av private kanalmeldinger ikke støttes, støttes oppbevaring av filer som deles i private kanaler.

**Trenger du en ny teameier?**

Hvis eieren av den private kanalen din forlater, kan du legge til en ny teameier via Teams Powershell.


- Gå [hit](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) for å installere Teams Powershell.

Her er cmdleten du trenger:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Hvis du vil ha mer informasjon om Teams Powershell, kan du se [Oversikt over Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
