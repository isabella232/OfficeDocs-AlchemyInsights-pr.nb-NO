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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Kontrollere informasjons innstillinger og deltakelses nivå i Teams

Hvis du vil tillate alle, inkludert innringede, eksterne og anonyme brukere, kan du bruke PowerShell til å utføre denne oppgaven for å **omgå den**. Her er et eksempel på hvordan du endrer den globale møte policyen for organisasjonen.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Denne cmdleten krever for øyeblikket bruk av Skype for Business PowerShell-modul. Hvis du vil konfigurere for å bruke denne cmdleten, kan du se [Behandle policyer via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Når du har konfigurert en policy, må du bruke den på brukere. Hvis du endret den globale policyen, vil den automatisk gjelde for brukere. For enhver policy endring må du vente minst **4 timer opptil 24 timer** før policyene trer i kraft. 

Pass på å se gjennom dokumentasjonen nedenfor før du gjør disse endringene for å forstå nøyaktig hva dette tillater.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Lære om retnings linjer for informasjons kontroller for Teams

Disse innstillingene styrer hvilke møte deltakere som venter på data før de blir lagt til møtet og deltakelses nivået som er tillatt i et møte. Du kan bruke PowerShell til å oppdatere innstillingene for møte policy som ennå ikke er implementert (merket "kommer snart") i administrasjons senteret for Teams. Se nedenfor for et eksempel på PowerShell-cmdlet som tillater alle brukere å hoppe over den aktuelle informasjons filen.

- [Gi tilgang personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) er en per Organizer-policy som styrer om personer skal bli med i et møte direkte eller vente i den, før de lagt av en godkjent bruker.

- [Tillat at anonyme personer kan starte et møte](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) er en per Organizer-policy som styrer om anonyme personer, inkludert B2B og Forbunds brukere, kan bli med i brukerens møte uten en godkjent bruker fra organisasjonen som deltar.

- [Tillat at innringings brukere kan hoppe over informasjons](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) er en per-arrangør-policy som styrer om personer som ringer inn via telefon, skal bli med i møtet direkte eller vente i informasjons delen uavhengig av innstillingen for **automatisk gi tilgang av personer** .

- [Tillat at arrangører overstyrer informasjons innstillinger](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) er en per Organizer-policy som styrer om møte arrangøren kan overstyre informasjons innstillingene som en administrator angir i **automatisk gi tilgang-personer** og **tillate at innringings brukere omgår data** når de planlegger et nytt møte.

**Obs!** Les [Behandle møte policyer i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for å få en fullstendig oversikt over møte retnings linjene i Microsoft Teams.
