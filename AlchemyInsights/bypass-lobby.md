---
title: Hoppe over lobbyen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820043"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="b995f-102">Kontrollere lobbyinnstillinger og deltakelsesnivå i Teams</span><span class="sxs-lookup"><span data-stu-id="b995f-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="b995f-103">Hvis du vil tillate at alle, inkludert innringings-, eksterne og anonyme brukere, kan **omgå lobbyen,** kan du bruke PowerShell til å utføre denne oppgaven.</span><span class="sxs-lookup"><span data-stu-id="b995f-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="b995f-104">Her er et eksempel på endring av den globale møtepolicyen for organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="b995f-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="b995f-105">Denne cmdleten krever for øyeblikket bruk av Skype for Business PowerShell-modulen.</span><span class="sxs-lookup"><span data-stu-id="b995f-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="b995f-106">Hvis du vil konfigurere deg til å bruke denne cmdleten, kan du [se Administrere policyer via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="b995f-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="b995f-107">Når du har konfigurert en policy, må du bruke den for brukere. Eller, hvis du har endret den globale policyen, vil den automatisk gjelde for brukere.</span><span class="sxs-lookup"><span data-stu-id="b995f-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="b995f-108">For policyendringer må du vente minst fire timer opptil **24 timer** før policyene trer i kraft.</span><span class="sxs-lookup"><span data-stu-id="b995f-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="b995f-109">Pass på å se gjennom dokumentasjonen nedenfor før du gjør disse endringene for å forstå nøyaktig hva dette tillater.</span><span class="sxs-lookup"><span data-stu-id="b995f-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="b995f-110">Forstå policykontroller for Teams-møtelobby</span><span class="sxs-lookup"><span data-stu-id="b995f-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="b995f-111">Disse innstillingene kontrollerer hvilke møtedeltakere som venter i lobbyen før de blir tatt opp til møtet, og hvor mye de kan delta i et møte.</span><span class="sxs-lookup"><span data-stu-id="b995f-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="b995f-112">Du kan bruke PowerShell til å oppdatere innstillinger for møtepolicyer som ennå ikke er implementert (merket «kommer snart») i administrasjonssenteret for Teams.</span><span class="sxs-lookup"><span data-stu-id="b995f-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="b995f-113">Se nedenfor for et eksempel på PowerShell-cmdlet som lar alle brukere omgå lobbyen.</span><span class="sxs-lookup"><span data-stu-id="b995f-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="b995f-114">[Automatisk tilgang til personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) er en policy per arrangør som styrer om personer blir med i et møte direkte eller venter i lobbyen til de slippes inn av en godkjent bruker.</span><span class="sxs-lookup"><span data-stu-id="b995f-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="b995f-115">Tillat [anonyme](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) personer å starte et møte er en policy per arrangør som styrer om anonyme personer, inkludert B2B og brukere i forbund, kan bli med i brukerens møte uten en godkjent bruker fra organisasjonen som deltar.</span><span class="sxs-lookup"><span data-stu-id="b995f-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="b995f-116">Tillat [innringingsbrukere](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) å hoppe over lobbyen **(kommer** snart) er en policy per arrangør som styrer om personer  som ringer inn via telefon, blir med i møtet direkte eller venter i lobbyen, uavhengig av innstillingen Tillat personer automatisk.</span><span class="sxs-lookup"><span data-stu-id="b995f-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="b995f-117">Tillat at arrangører overstyrer lobbyinnstillinger [(kommer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **snart)** er en policy per arrangør som  styrer om møtearrangøren kan overstyre lobbyinnstillingene som en administrator angir i Tillat innringingsbrukere automatisk å hoppe over **lobbyen** når de planlegger et nytt møte.</span><span class="sxs-lookup"><span data-stu-id="b995f-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="b995f-118">**Obs!** Les [Behandle møtepolicyer i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for å få en fullstendig oversikt over microsoft Teams-møtepolicyer.</span><span class="sxs-lookup"><span data-stu-id="b995f-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
