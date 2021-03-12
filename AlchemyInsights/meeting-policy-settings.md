---
title: Policyinnstillinger for møte
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
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704615"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="515b7-102">Administrere møtepolicyer i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="515b7-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="515b7-103">**Obs! Det kan ta opptil 24 timer før policyendringer trer i kraft for brukerne.**</span><span class="sxs-lookup"><span data-stu-id="515b7-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="515b7-104">Du kan kanskje ikke gjøre endringer i nylig opprettede policyer umiddelbart. vent i fire timer og prøv å endre en nylig opprettet policy på nytt.</span><span class="sxs-lookup"><span data-stu-id="515b7-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="515b7-105">Møtepolicyer brukes til å kontrollere funksjonene som er tilgjengelige for møtedeltakere for møter som planlegges av brukere i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="515b7-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="515b7-106">Noen funksjoner i møtepolicyer kan ikke implementeres i administrasjonssenteret for Teams ennå (disse er merket «kommer snart» i dokumentasjonen).</span><span class="sxs-lookup"><span data-stu-id="515b7-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="515b7-107">I dette tilfellet, eller hvis du får en feilmelding som for eksempel «Vi kan ikke oppdatere policyen akkurat nå, men prøv på nytt senere» i administrasjonssenteret for Microsoft Teams, anbefaler vi at du bruker PowerShell til å opprette eller endre møtepolicyer i Teams.</span><span class="sxs-lookup"><span data-stu-id="515b7-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="515b7-108">Hvis du vil ha mer informasjon om møtepolicyer, kan du se følgende ressurser:</span><span class="sxs-lookup"><span data-stu-id="515b7-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="515b7-109">Hvis du vil vite mer om å opprette policyer, gjøre endringer og tilordne brukere til policyen, kan du se [Administrere møtepolicyer i Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="515b7-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="515b7-110">Hvis du vil gjøre policyendringer ved hjelp av PowerShell-cmdleter, kan du se Oversikt over [Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="515b7-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="515b7-111">Du må bruke [Skype for Business PowerShell-modulen](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for teams møtepolicyer.</span><span class="sxs-lookup"><span data-stu-id="515b7-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="515b7-112">Se gjennom [cmdlet-dokumentasjonen for \*-CsTeamsMeetingPolicy-cmdleter](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="515b7-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

