---
title: Policyinnstillinger for møte
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
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704615"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Administrere møtepolicyer i Microsoft Teams

**Obs! Det kan ta opptil 24 timer før policyendringer trer i kraft for brukerne.** Du kan kanskje ikke gjøre endringer i nylig opprettede policyer umiddelbart. vent i fire timer og prøv å endre en nylig opprettet policy på nytt.

Møtepolicyer brukes til å kontrollere funksjonene som er tilgjengelige for møtedeltakere for møter som planlegges av brukere i organisasjonen. Noen funksjoner i møtepolicyer kan ikke implementeres i administrasjonssenteret for Teams ennå (disse er merket «kommer snart» i dokumentasjonen). I dette tilfellet, eller hvis du får en feilmelding som for eksempel «Vi kan ikke oppdatere policyen akkurat nå, men prøv på nytt senere» i administrasjonssenteret for Microsoft Teams, anbefaler vi at du bruker PowerShell til å opprette eller endre møtepolicyer i Teams. 

Hvis du vil ha mer informasjon om møtepolicyer, kan du se følgende ressurser:

- Hvis du vil vite mer om å opprette policyer, gjøre endringer og tilordne brukere til policyen, kan du se [Administrere møtepolicyer i Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Hvis du vil gjøre policyendringer ved hjelp av PowerShell-cmdleter, kan du se Oversikt over [Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Du må bruke [Skype for Business PowerShell-modulen](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for teams møtepolicyer. 
    - Se gjennom [cmdlet-dokumentasjonen for *-CsTeamsMeetingPolicy-cmdleter](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for mer informasjon.

