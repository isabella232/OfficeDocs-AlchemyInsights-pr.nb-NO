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
ms.openlocfilehash: 729fc5d4213acbbdf74a9d07adacb42b34170717
ms.sourcegitcommit: ffbeb72c9199ab4ebcb0f1ad443ed3e2f4950efc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/23/2019
ms.locfileid: "37637786"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="bbeb5-102">Kontrollér innstillingene for lobbyen og nivå for deltakelse</span><span class="sxs-lookup"><span data-stu-id="bbeb5-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="bbeb5-103">Hvis du ønsker å tillate alle, inkludert dial-in, eksterne og anonyme brukere å omgå lobbyen, kan du bruke PowerShell til å gjøre det.</span><span class="sxs-lookup"><span data-stu-id="bbeb5-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby, you can use PowerShell to do it.</span></span> <span data-ttu-id="bbeb5-104">Her er et eksempel på hvordan du endrer den globale møte policyen for organisasjonen:</span><span class="sxs-lookup"><span data-stu-id="bbeb5-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="bbeb5-105">Denne cmdleten krever for øyeblikket bruk av Skype for Business PowerShell-modulen.</span><span class="sxs-lookup"><span data-stu-id="bbeb5-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="bbeb5-106">For å få oppsett til å bruke denne cmdleten, kan du sjekke ut administrerende policyer via PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bbeb5-106">To get setup to use this cmdlet, check out Managing policies via PowerShell.</span></span>

<span data-ttu-id="bbeb5-107">Du kan sette opp en ny policy, som du deretter må bruke den til brukerne.</span><span class="sxs-lookup"><span data-stu-id="bbeb5-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="bbeb5-108">Hvis du endrer den globale policyen, vil den automatisk gjelde for brukerne.</span><span class="sxs-lookup"><span data-stu-id="bbeb5-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="bbeb5-109">For alle politikk endre du nød å vent det vil si 4 timene og til 24 timene for det politiet å tre i kraft.</span><span class="sxs-lookup"><span data-stu-id="bbeb5-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="bbeb5-110">Husk å se gjennom dokumentasjonen nedenfor før du gjør disse endringene for å forstå nøyaktig hva dette tillater.</span><span class="sxs-lookup"><span data-stu-id="bbeb5-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="bbeb5-111">Forstå Teams-policy kontroller for gruppemøte</span><span class="sxs-lookup"><span data-stu-id="bbeb5-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="bbeb5-112">[Automatisk innrømme at personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) er en policy for hver arrangør som kontrollerer om personer blir med i et møte direkte eller venter i vestibylen til de blir tatt opp av en godkjent bruker.</span><span class="sxs-lookup"><span data-stu-id="bbeb5-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="bbeb5-113">[Tillate at anonyme personer starter et møte](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , er en policy for hver arrangør som kontrollerer om anonyme personer, inkludert B2B-og Federated brukere, kan delta i brukerens møte uten en godkjent bruker fra organisasjonen som er tilstede.</span><span class="sxs-lookup"><span data-stu-id="bbeb5-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="bbeb5-114">[Tillat eksterne brukere å omgå lobbyen](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) er en per-arrangør politikk som styrer om folk som ringer inn via telefon delta i møtet direkte eller vente i lobbyen uavhengig av **automatisk innrømme folk** innstillingen.</span><span class="sxs-lookup"><span data-stu-id="bbeb5-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="bbeb5-115">[La arrangørene overstyre lobby innstillingene](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) er en policy for hver arrangør som kontrollerer om møtearrangøren kan overstyre lobby innstillingene som en administrator har angitt i automatisk å **innrømme personer** og **tillate ekstern pålogging brukere å omgå lobbyen** når de planlegger et nytt møte.</span><span class="sxs-lookup"><span data-stu-id="bbeb5-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="bbeb5-116">**Merk:** Les [Behandle møte policyer i Teams for å](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) se en fullstendig oversikt over retningslinjene for Microsoft Teams-møte.</span><span class="sxs-lookup"><span data-stu-id="bbeb5-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
