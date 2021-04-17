---
title: Innstillinger for møtepolicy
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825452"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Administrere møtepolicyer i Microsoft Teams

**Obs! Det kan ta opptil 24 timer før policyendringer trer i kraft for brukere.** Det kan hende du ikke kan gjøre endringer i nylig opprettede policyer umiddelbart. vent i fire timer, og prøv å endre en nyopprettet policy på nytt.

Møtepolicyer brukes til å kontrollere funksjonene som er tilgjengelige for møtedeltakere for møter som er planlagt av brukere i organisasjonen. Noen funksjoner i møtepolicyer er kanskje ikke implementert i administrasjonssenteret for Teams ennå (disse er merket «kommer snart» i dokumentasjonen). I dette tilfellet, eller hvis du får en feilmelding som «Vi kan ikke oppdatere policyen akkurat nå, men prøv det på nytt senere» i administrasjonssenteret for Microsoft Teams, anbefaler vi at du bruker PowerShell til å opprette eller endre Teams-møtepolicyer. 

Hvis du vil ha mer informasjon om møtepolicyer, kan du se følgende ressurser:

- Hvis du vil lære om hvordan du oppretter policyer, gjør endringer og tilordner brukere til policyen, kan du se [Administrere møtepolicyer i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Hvis du vil gjøre policyendringer ved hjelp av PowerShell-cmdleter, kan du se [Oversikt over Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Du må bruke [PowerShell-modulen for Skype for Business](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for teams møtepolicyer. 
    - Se gjennom [cmdletene for CSTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for mer informasjon.

