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
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925174"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Behandle møtepolicyer i Microsoft Teams

**Obs! Det kan ta opptil 24 timer før policyendringer trer i kraft for brukere.** Det kan hende du ikke kan gjøre endringer i nylig opprettede policyer umiddelbart. vent i fire timer, og prøv å endre en nyopprettet policy på nytt.

Møtepolicyer brukes til å kontrollere funksjonene som er tilgjengelige for møtedeltakere for møter som er planlagt av brukere i organisasjonen. Enkelte funksjoner i møtepolicyer er kanskje ikke implementert i Teams administrasjonssenteret ennå (disse er merket «kommer snart» i dokumentasjonen). I dette tilfellet, eller hvis du får en feilmelding som «Vi kan ikke oppdatere policyen akkurat nå, men prøv den på nytt senere» i administrasjonssenteret for Microsoft Teams, anbefaler vi at du bruker PowerShell til å opprette eller endre Teams møtepolicyer. 

Hvis du vil ha mer informasjon om møtepolicyer, kan du se følgende ressurser:

- Hvis du vil lære mer om hvordan du oppretter policyer, gjør endringer og tilordner brukere til policyen, kan du se [Administrere møtepolicyer i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Hvis du vil gjøre policyendringer ved hjelp av PowerShell-cmdleter, [kan du Teams PowerShell-oversikt](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Du må bruke [PowerShell-Skype for Business for](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) å Teams møtepolicyer. 
    - Se gjennom [cmdletene for CSTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for mer informasjon.

