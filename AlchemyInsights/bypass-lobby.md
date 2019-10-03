---
title: Omkjøringsvei lobby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376753"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="c4527-102">Kontrollér innstillingene for lobbyen og nivå for deltakelse</span><span class="sxs-lookup"><span data-stu-id="c4527-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="c4527-103">Disse innstillingene kontrollerer hvilke møtedeltakere som venter i vestibylen før de blir tatt opp på møtet og nivået på deltakelsen de er tillatt i et møte.</span><span class="sxs-lookup"><span data-stu-id="c4527-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="c4527-104">Du kan bruke PowerShell til å oppdatere innstillinger for møte policy som ennå ikke er implementert (merket "kommer snart") i Teams Administrasjonssenter.</span><span class="sxs-lookup"><span data-stu-id="c4527-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="c4527-105">Se nedenfor for et eksempel PowerShell cmdlet som gjør at alle brukere til å omgå lobbyen.</span><span class="sxs-lookup"><span data-stu-id="c4527-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="c4527-106">[Automatisk innrømme at personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) er en policy for hver arrangør som kontrollerer om personer blir med i et møte direkte eller venter i vestibylen til de blir tatt opp av en godkjent bruker.</span><span class="sxs-lookup"><span data-stu-id="c4527-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="c4527-107">[Tillate at anonyme personer starter et møte](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , er en policy for hver arrangør som kontrollerer om anonyme personer, inkludert B2B-og Federated brukere, kan delta i brukerens møte uten en godkjent bruker fra organisasjonen som er tilstede.</span><span class="sxs-lookup"><span data-stu-id="c4527-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="c4527-108">[Tillat eksterne brukere å omgå lobbyen](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) er en per-arrangør politikk som styrer om folk som ringer inn via telefon delta i møtet direkte eller vente i lobbyen uavhengig av **automatisk innrømme folk** innstillingen.</span><span class="sxs-lookup"><span data-stu-id="c4527-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="c4527-109">[La arrangørene overstyre lobby innstillingene](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) er en policy for hver arrangør som kontrollerer om møtearrangøren kan overstyre lobby innstillingene som en administrator har angitt i automatisk å **innrømme personer** og **tillate ekstern pålogging brukere å omgå lobbyen** når de planlegger et nytt møte.</span><span class="sxs-lookup"><span data-stu-id="c4527-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="c4527-110">**Merk:** Les [Behandle møte policyer i Teams for å](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) se en fullstendig oversikt over retningslinjene for Microsoft Teams-møte.</span><span class="sxs-lookup"><span data-stu-id="c4527-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="c4527-111">**PowerShell-eksempel**</span><span class="sxs-lookup"><span data-stu-id="c4527-111">**PowerShell example**</span></span>

<span data-ttu-id="c4527-112">Hvis du ønsker å tillate alle, inkludert eksterne eller anonyme brukere, å omgå lobbyen, kan du også bruke PowerShell til å utføre denne oppgaven.</span><span class="sxs-lookup"><span data-stu-id="c4527-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="c4527-113">Her er et eksempel på hvordan du endrer den globale møte policyen for organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="c4527-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="c4527-114">(Husk å se gjennom dokumentasjonen ovenfor før du gjør disse endringene for å forstå nøyaktig hva dette tillater.)</span><span class="sxs-lookup"><span data-stu-id="c4527-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="c4527-115">Set-CsTeamsMeetingPolicy-identitet global-AutoAdmittedUsers "alle"-AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="c4527-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="c4527-116">Hvis du vil ha mer informasjon, se [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="c4527-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
