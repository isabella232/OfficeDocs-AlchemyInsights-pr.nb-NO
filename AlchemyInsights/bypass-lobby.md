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
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889091"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="61c87-102">Kontrollér innstillingene for lobbyen og nivået for deltakelse i Teams</span><span class="sxs-lookup"><span data-stu-id="61c87-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="61c87-103">Hvis du vil tillate alle, inkludert eksterne, eksterne og anonyme brukere, å **omgå vestibylen**, bruker du PowerShell til å utføre denne oppgaven.</span><span class="sxs-lookup"><span data-stu-id="61c87-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="61c87-104">Her er et eksempel på hvordan du endrer den globale møte policyen for organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="61c87-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="61c87-105">Denne cmdleten krever for øyeblikket bruk av Skype for Business PowerShell-modulen.</span><span class="sxs-lookup"><span data-stu-id="61c87-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="61c87-106">For å få satt opp til å bruke denne cmdleten, kan du sjekke ut [administrerende policyer via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="61c87-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="61c87-107">Når du har konfigurert en policy, må du bruke den på brukere. eller, hvis du endret den globale policyen, vil den automatisk gjelde for brukerne.</span><span class="sxs-lookup"><span data-stu-id="61c87-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="61c87-108">For alle politikk endre, du nød å vent det vil si **4 timene til 24 timene** for det politiet å tre i kraft.</span><span class="sxs-lookup"><span data-stu-id="61c87-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="61c87-109">Husk å se gjennom dokumentasjonen nedenfor før du gjør disse endringene for å forstå nøyaktig hva dette tillater.</span><span class="sxs-lookup"><span data-stu-id="61c87-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="61c87-110">Forstå Teams-policy kontroller for gruppemøte</span><span class="sxs-lookup"><span data-stu-id="61c87-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="61c87-111">Disse innstillingene kontrollerer hvilke møtedeltakere som venter i vestibylen før de blir tatt opp på møtet og nivået på deltakelsen de er tillatt i et møte.</span><span class="sxs-lookup"><span data-stu-id="61c87-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="61c87-112">Du kan bruke PowerShell til å oppdatere innstillinger for møte policy som ennå ikke er implementert (merket "kommer snart") i Teams Administrasjonssenter.</span><span class="sxs-lookup"><span data-stu-id="61c87-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="61c87-113">Se nedenfor for et eksempel PowerShell cmdlet som gjør at alle brukere til å omgå lobbyen.</span><span class="sxs-lookup"><span data-stu-id="61c87-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="61c87-114">[Automatisk innrømme at personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) er en policy for hver arrangør som kontrollerer om personer blir med i et møte direkte eller venter i vestibylen til de blir tatt opp av en godkjent bruker.</span><span class="sxs-lookup"><span data-stu-id="61c87-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="61c87-115">[Tillate at anonyme personer starter et møte](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , er en policy for hver arrangør som kontrollerer om anonyme personer, inkludert B2B-og Federated brukere, kan delta i brukerens møte uten en godkjent bruker fra organisasjonen som er tilstede.</span><span class="sxs-lookup"><span data-stu-id="61c87-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="61c87-116">[Tillat eksterne brukere å omgå lobbyen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) er en per-arrangør politikk som styrer om folk som ringer inn via telefon delta i møtet direkte eller vente i lobbyen uavhengig av **automatisk innrømme folk** innstillingen.</span><span class="sxs-lookup"><span data-stu-id="61c87-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="61c87-117">[La arrangørene overstyre lobby innstillingene](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) er en policy for hver arrangør som kontrollerer om møtearrangøren kan overstyre lobby innstillingene som en administrator har angitt i automatisk å **innrømme personer** og **tillate at eksterne brukere omgår lobbyen** når de planlegger et nytt møte.</span><span class="sxs-lookup"><span data-stu-id="61c87-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="61c87-118">**Merk:** Les [Behandle møte policyer i Teams for å](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) se en fullstendig oversikt over retningslinjene for Microsoft Teams-møte.</span><span class="sxs-lookup"><span data-stu-id="61c87-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
