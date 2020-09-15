---
title: Omgå informasjons
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
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684959"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="25aad-102">Kontrollere informasjons innstillinger og deltakelses nivå i Teams</span><span class="sxs-lookup"><span data-stu-id="25aad-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="25aad-103">Hvis du vil tillate alle, inkludert innringede, eksterne og anonyme brukere, kan du bruke PowerShell til å utføre denne oppgaven for å **omgå den**.</span><span class="sxs-lookup"><span data-stu-id="25aad-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="25aad-104">Her er et eksempel på hvordan du endrer den globale møte policyen for organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="25aad-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="25aad-105">Denne cmdleten krever for øyeblikket bruk av Skype for Business PowerShell-modul.</span><span class="sxs-lookup"><span data-stu-id="25aad-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="25aad-106">Hvis du vil konfigurere for å bruke denne cmdleten, kan du se [Behandle policyer via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="25aad-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="25aad-107">Når du har konfigurert en policy, må du bruke den på brukere. Hvis du endret den globale policyen, vil den automatisk gjelde for brukere.</span><span class="sxs-lookup"><span data-stu-id="25aad-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="25aad-108">For enhver policy endring må du vente minst **4 timer opptil 24 timer** før policyene trer i kraft.</span><span class="sxs-lookup"><span data-stu-id="25aad-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="25aad-109">Pass på å se gjennom dokumentasjonen nedenfor før du gjør disse endringene for å forstå nøyaktig hva dette tillater.</span><span class="sxs-lookup"><span data-stu-id="25aad-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="25aad-110">Lære om retnings linjer for informasjons kontroller for Teams</span><span class="sxs-lookup"><span data-stu-id="25aad-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="25aad-111">Disse innstillingene styrer hvilke møte deltakere som venter på data før de blir lagt til møtet og deltakelses nivået som er tillatt i et møte.</span><span class="sxs-lookup"><span data-stu-id="25aad-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="25aad-112">Du kan bruke PowerShell til å oppdatere innstillingene for møte policy som ennå ikke er implementert (merket "kommer snart") i administrasjons senteret for Teams.</span><span class="sxs-lookup"><span data-stu-id="25aad-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="25aad-113">Se nedenfor for et eksempel på PowerShell-cmdlet som tillater alle brukere å hoppe over den aktuelle informasjons filen.</span><span class="sxs-lookup"><span data-stu-id="25aad-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="25aad-114">[Gi tilgang personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) er en per Organizer-policy som styrer om personer skal bli med i et møte direkte eller vente i den, før de lagt av en godkjent bruker.</span><span class="sxs-lookup"><span data-stu-id="25aad-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="25aad-115">[Tillat at anonyme personer kan starte et møte](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) er en per Organizer-policy som styrer om anonyme personer, inkludert B2B og Forbunds brukere, kan bli med i brukerens møte uten en godkjent bruker fra organisasjonen som deltar.</span><span class="sxs-lookup"><span data-stu-id="25aad-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="25aad-116">[Tillat at innringings brukere kan hoppe over informasjons](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) er en per-arrangør-policy som styrer om personer som ringer inn via telefon, skal bli med i møtet direkte eller vente i informasjons delen uavhengig av innstillingen for **automatisk gi tilgang av personer** .</span><span class="sxs-lookup"><span data-stu-id="25aad-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="25aad-117">[Tillat at arrangører overstyrer informasjons innstillinger](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) er en per Organizer-policy som styrer om møte arrangøren kan overstyre informasjons innstillingene som en administrator angir i **automatisk gi tilgang-personer** og **tillate at innringings brukere omgår data** når de planlegger et nytt møte.</span><span class="sxs-lookup"><span data-stu-id="25aad-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="25aad-118">**Obs!** Les [Behandle møte policyer i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for å få en fullstendig oversikt over møte retnings linjene i Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="25aad-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
