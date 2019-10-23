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
# <a name="control-lobby-settings-and-level-of-participation"></a>Kontrollér innstillingene for lobbyen og nivå for deltakelse

Hvis du ønsker å tillate alle, inkludert dial-in, eksterne og anonyme brukere å omgå lobbyen, kan du bruke PowerShell til å gjøre det. Her er et eksempel på hvordan du endrer den globale møte policyen for organisasjonen:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Denne cmdleten krever for øyeblikket bruk av Skype for Business PowerShell-modulen. For å få oppsett til å bruke denne cmdleten, kan du sjekke ut administrerende policyer via PowerShell.

Du kan sette opp en ny policy, som du deretter må bruke den til brukerne. Hvis du endrer den globale policyen, vil den automatisk gjelde for brukerne. For alle politikk endre du nød å vent det vil si 4 timene og til 24 timene for det politiet å tre i kraft.

Husk å se gjennom dokumentasjonen nedenfor før du gjør disse endringene for å forstå nøyaktig hva dette tillater.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Forstå Teams-policy kontroller for gruppemøte

- [Automatisk innrømme at personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) er en policy for hver arrangør som kontrollerer om personer blir med i et møte direkte eller venter i vestibylen til de blir tatt opp av en godkjent bruker.

- [Tillate at anonyme personer starter et møte](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , er en policy for hver arrangør som kontrollerer om anonyme personer, inkludert B2B-og Federated brukere, kan delta i brukerens møte uten en godkjent bruker fra organisasjonen som er tilstede.

- [Tillat eksterne brukere å omgå lobbyen](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) er en per-arrangør politikk som styrer om folk som ringer inn via telefon delta i møtet direkte eller vente i lobbyen uavhengig av **automatisk innrømme folk** innstillingen.

- [La arrangørene overstyre lobby innstillingene](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) er en policy for hver arrangør som kontrollerer om møtearrangøren kan overstyre lobby innstillingene som en administrator har angitt i automatisk å **innrømme personer** og **tillate ekstern pålogging brukere å omgå lobbyen** når de planlegger et nytt møte.

**Merk:** Les [Behandle møte policyer i Teams for å](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) se en fullstendig oversikt over retningslinjene for Microsoft Teams-møte.
