---
title: Innstillinger for møte policy
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
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794343"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Behandle møte policyer i Microsoft Teams

**Obs! det kan ha opptil 24 timer før policy endringer trer i kraft for brukere.** Det kan hende du ikke kan gjøre endringer i nylig opprettede policyer umiddelbart. Vent 4 timer, og prøv å endre en nylig opprettet policy på nytt.

Møte policyer brukes til å kontrollere funksjonene som er tilgjengelige for møte deltakere for møter som er planlagt av brukere i organisasjonen. Noen funksjoner for møte policyer er kanskje ikke implementert i administrasjons senteret for Teams ennå (disse er merket "kommer snart" i dokumentasjonen). I dette tilfellet, hvis du får en feil melding om at vi ikke kan oppdatere policyen, men prøv den på nytt senere i administrasjons senteret for Microsoft Teams, anbefaler vi at du bruker PowerShell til å opprette eller endre teamets møte retnings linjer. 

Hvis du vil ha mer informasjon om møte policyer, kan du se følgende ressurser:

- Hvis du vil lære om hvordan du oppretter policyer, gjør endringer og tilordner brukere til policyen, kan du se [Behandle møte policyer i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Se [Teams PowerShell-oversikt](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)for å gjøre policy endringer ved hjelp av PowerShell-cmdleter. 
    - Du må bruke [Skype for Business PowerShell-modulen](https://www.microsoft.com/download/details.aspx?id=39366) for Teams-policyer. 
    - Se gjennom [dokumentasjonen for *-CsTeamsMeetingPolicy-cmdleten](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for mer informasjon.

