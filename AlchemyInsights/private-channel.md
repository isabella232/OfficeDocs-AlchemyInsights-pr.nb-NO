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
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="9d5ab-102">Private kanaler i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9d5ab-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="9d5ab-103">Private kanaler er en ny funksjon i Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="9d5ab-104">Vær oppmerksom på at private kanaler ikke kan konverteres fra standardkanaler eller omvendt.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="9d5ab-105">Hvis du vil ha mer informasjon om private kanaler, for eksempel informasjon om [oppretting og medlemskap](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) i private kanaler og [SharePoint-områder](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)i private kanaler, kan du se Private kanaler i Microsoft [Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="9d5ab-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="9d5ab-106">**Merk:** Fordi konfigurasjon for oppbevaring av private kanalmeldinger ennå ikke støttes, vil ikke leietakere med oppbevaringspolicyer aktivert ha private kanaler aktivert som standard.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="9d5ab-107">Private kanaler kan aktiveres i teams administrasjonssenter.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="9d5ab-108">Vær også oppmerksom på at selv om oppbevaring av private kanalmeldinger ikke støttes, støttes oppbevaring av filer som deles i private kanaler.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="9d5ab-109">**Trenger du en ny teameier?**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-109">**Need a new team owner?**</span></span>

<span data-ttu-id="9d5ab-110">Hvis eieren av den private kanalen din forlater, kan du legge til en ny teameier via Teams Powershell.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="9d5ab-111">Gå [hit](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) for å installere Teams Powershell.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="9d5ab-112">Her er cmdleten du trenger:</span><span class="sxs-lookup"><span data-stu-id="9d5ab-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="9d5ab-113">Hvis du vil ha mer informasjon om Teams Powershell, kan du se [Oversikt over Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="9d5ab-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
