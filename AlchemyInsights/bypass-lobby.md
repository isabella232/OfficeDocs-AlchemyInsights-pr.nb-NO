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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Kontrollér innstillingene for lobbyen og nivået for deltakelse i Teams

Hvis du vil tillate alle, inkludert eksterne, eksterne og anonyme brukere, å **omgå vestibylen**, bruker du PowerShell til å utføre denne oppgaven. Her er et eksempel på hvordan du endrer den globale møte policyen for organisasjonen.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Denne cmdleten krever for øyeblikket bruk av Skype for Business PowerShell-modulen. For å få satt opp til å bruke denne cmdleten, kan du sjekke ut [administrerende policyer via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Når du har konfigurert en policy, må du bruke den på brukere. eller, hvis du endret den globale policyen, vil den automatisk gjelde for brukerne. For alle politikk endre, du nød å vent det vil si **4 timene til 24 timene** for det politiet å tre i kraft. 

Husk å se gjennom dokumentasjonen nedenfor før du gjør disse endringene for å forstå nøyaktig hva dette tillater.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Forstå Teams-policy kontroller for gruppemøte

Disse innstillingene kontrollerer hvilke møtedeltakere som venter i vestibylen før de blir tatt opp på møtet og nivået på deltakelsen de er tillatt i et møte. Du kan bruke PowerShell til å oppdatere innstillinger for møte policy som ennå ikke er implementert (merket "kommer snart") i Teams Administrasjonssenter. Se nedenfor for et eksempel PowerShell cmdlet som gjør at alle brukere til å omgå lobbyen.

- [Automatisk innrømme at personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) er en policy for hver arrangør som kontrollerer om personer blir med i et møte direkte eller venter i vestibylen til de blir tatt opp av en godkjent bruker.

- [Tillate at anonyme personer starter et møte](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , er en policy for hver arrangør som kontrollerer om anonyme personer, inkludert B2B-og Federated brukere, kan delta i brukerens møte uten en godkjent bruker fra organisasjonen som er tilstede.

- [Tillat eksterne brukere å omgå lobbyen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) er en per-arrangør politikk som styrer om folk som ringer inn via telefon delta i møtet direkte eller vente i lobbyen uavhengig av **automatisk innrømme folk** innstillingen.

- [La arrangørene overstyre lobby innstillingene](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) er en policy for hver arrangør som kontrollerer om møtearrangøren kan overstyre lobby innstillingene som en administrator har angitt i automatisk å **innrømme personer** og **tillate at eksterne brukere omgår lobbyen** når de planlegger et nytt møte.

**Merk:** Les [Behandle møte policyer i Teams for å](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) se en fullstendig oversikt over retningslinjene for Microsoft Teams-møte.
