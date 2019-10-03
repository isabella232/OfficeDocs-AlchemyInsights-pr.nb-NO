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
# <a name="control-lobby-settings-and-level-of-participation"></a>Kontrollér innstillingene for lobbyen og nivå for deltakelse

Disse innstillingene kontrollerer hvilke møtedeltakere som venter i vestibylen før de blir tatt opp på møtet og nivået på deltakelsen de er tillatt i et møte. Du kan bruke PowerShell til å oppdatere innstillinger for møte policy som ennå ikke er implementert (merket "kommer snart") i Teams Administrasjonssenter.  Se nedenfor for et eksempel PowerShell cmdlet som gjør at alle brukere til å omgå lobbyen.  

- [Automatisk innrømme at personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) er en policy for hver arrangør som kontrollerer om personer blir med i et møte direkte eller venter i vestibylen til de blir tatt opp av en godkjent bruker.

- [Tillate at anonyme personer starter et møte](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , er en policy for hver arrangør som kontrollerer om anonyme personer, inkludert B2B-og Federated brukere, kan delta i brukerens møte uten en godkjent bruker fra organisasjonen som er tilstede.

- [Tillat eksterne brukere å omgå lobbyen](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) er en per-arrangør politikk som styrer om folk som ringer inn via telefon delta i møtet direkte eller vente i lobbyen uavhengig av **automatisk innrømme folk** innstillingen.

- [La arrangørene overstyre lobby innstillingene](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) er en policy for hver arrangør som kontrollerer om møtearrangøren kan overstyre lobby innstillingene som en administrator har angitt i automatisk å **innrømme personer** og **tillate ekstern pålogging brukere å omgå lobbyen** når de planlegger et nytt møte.

**Merk:** Les [Behandle møte policyer i Teams for å](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) se en fullstendig oversikt over retningslinjene for Microsoft Teams-møte. 


**PowerShell-eksempel**

Hvis du ønsker å tillate alle, inkludert eksterne eller anonyme brukere, å omgå lobbyen, kan du også bruke PowerShell til å utføre denne oppgaven.  Her er et eksempel på hvordan du endrer den globale møte policyen for organisasjonen.   

(Husk å se gjennom dokumentasjonen ovenfor før du gjør disse endringene for å forstå nøyaktig hva dette tillater.)

Set-CsTeamsMeetingPolicy-identitet global-AutoAdmittedUsers "alle"-AllowPSTNUsersToBypassLobby $True

Hvis du vil ha mer informasjon, se [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
