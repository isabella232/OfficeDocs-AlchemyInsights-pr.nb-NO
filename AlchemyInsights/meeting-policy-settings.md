---
title: Innstillinger for møtepolicy
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042853"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="e0af2-102">Administrere møtepolicyer i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e0af2-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="e0af2-103">**Merk: Det kan ta opptil 24 timer før policyendringer trer i kraft for brukerne.**</span><span class="sxs-lookup"><span data-stu-id="e0af2-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="e0af2-104">Du kan kanskje ikke gjøre endringer i nyopprettede policyer umiddelbart. vent 4 timer, og prøv å endre en nylig opprettet policy på nytt.</span><span class="sxs-lookup"><span data-stu-id="e0af2-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="e0af2-105">Møtepolicyer brukes til å kontrollere funksjonene som er tilgjengelige for møte deltakere for møter som er planlagt av brukere i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="e0af2-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="e0af2-106">Noen funksjoner i møtepolicyer kan ikke implementeres i Teams administrasjonssenter ennå (disse er merket "kommer snart" i dokumentasjonen).</span><span class="sxs-lookup"><span data-stu-id="e0af2-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="e0af2-107">I dette tilfellet, eller hvis du får en feil som "Vi kan ikke oppdatere policyen akkurat nå, men prøv det på nytt senere" i administrasjonssenteret for Microsoft Teams, anbefaler vi at du bruker PowerShell til å opprette eller endre teams møtepolicyer.</span><span class="sxs-lookup"><span data-stu-id="e0af2-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="e0af2-108">Hvis du vil ha mer informasjon om møtepolicyer, kan du se følgende ressurser:</span><span class="sxs-lookup"><span data-stu-id="e0af2-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="e0af2-109">Hvis du vil vite mer om hvordan du oppretter policyer, gjør endringer og tilordner brukere til policyen, kan du se [Administrere møtepolicyer i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="e0af2-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="e0af2-110">Hvis du vil gjøre endringer i retningslinjene ved hjelp av PowerShell-cmdleter, kan du se [Teams PowerShell-oversikt](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="e0af2-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="e0af2-111">Du må bruke [Skype for Business PowerShell-modulen](https://www.microsoft.com/download/details.aspx?id=39366) for teams-møtepolicyer.</span><span class="sxs-lookup"><span data-stu-id="e0af2-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="e0af2-112">Se gjennom [cmdleterdokumentasjonen \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) hvis du vil ha mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="e0af2-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

