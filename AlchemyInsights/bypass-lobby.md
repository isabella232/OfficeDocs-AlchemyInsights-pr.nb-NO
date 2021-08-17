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
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059605"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Kontroller lobbyinnstillinger og deltakelsesnivå i Teams

Hvis du vil tillate at alle, inkludert innringings-, eksterne og anonyme brukere, kan **omgå lobbyen,** kan du bruke PowerShell til å utføre denne oppgaven. Her er et eksempel på endring av den globale møtepolicyen for organisasjonen.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Denne cmdleten krever for øyeblikket bruk av Skype for Business PowerShell-modulen. Hvis du vil konfigurere deg til å bruke denne cmdleten, kan du [se Administrere policyer via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Når du har konfigurert en policy, må du bruke den for brukere. Eller, hvis du har endret den globale policyen, vil den automatisk gjelde for brukere. For policyendringer må du vente minst fire timer opptil **24 timer** før policyene trer i kraft. 

Pass på å se gjennom dokumentasjonen nedenfor før du gjør disse endringene for å forstå nøyaktig hva dette tillater.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Forstå Teams policykontroller i møtelobbyen

Disse innstillingene kontrollerer hvilke møtedeltakere som venter i lobbyen før de blir tatt opp til møtet, og hvor mye de kan delta i et møte. Du kan bruke PowerShell til å oppdatere innstillinger for møtepolicyer som ennå ikke er implementert (merket «kommer snart») i Teams administrasjonssenteret. Se nedenfor for et eksempel på PowerShell-cmdlet som lar alle brukere omgå lobbyen.

- [Automatisk tilgang til personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) er en policy per arrangør som styrer om personer blir med i et møte direkte eller venter i lobbyen til de slippes inn av en godkjent bruker.

- Tillat [anonyme](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) personer å starte et møte er en policy per arrangør som styrer om anonyme personer, inkludert B2B og brukere i forbund, kan bli med i brukerens møte uten en godkjent bruker fra organisasjonen som deltar.

- Tillat [innringingsbrukere](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) å hoppe over lobbyen **(kommer** snart) er en policy per arrangør som styrer om personer  som ringer inn via telefon, blir med i møtet direkte eller venter i lobbyen, uavhengig av innstillingen Tillat personer automatisk.

- Tillat at arrangører overstyrer lobbyinnstillinger [(kommer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **snart)** er en policy per arrangør som  styrer om møtearrangøren kan overstyre lobbyinnstillingene som en administrator angir i Tillat innringingsbrukere automatisk å hoppe over **lobbyen** når de planlegger et nytt møte.

**Obs!** Les [Behandle møtepolicyer i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for en fullstendig oversikt over Microsoft Teams møtepolicyer.
