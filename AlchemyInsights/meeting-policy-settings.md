---
title: Innstillinger for møtepolicy
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042853"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Administrere møtepolicyer i Microsoft Teams

**Merk: Det kan ta opptil 24 timer før policyendringer trer i kraft for brukerne.** Du kan kanskje ikke gjøre endringer i nyopprettede policyer umiddelbart. vent 4 timer, og prøv å endre en nylig opprettet policy på nytt.

Møtepolicyer brukes til å kontrollere funksjonene som er tilgjengelige for møte deltakere for møter som er planlagt av brukere i organisasjonen. Noen funksjoner i møtepolicyer kan ikke implementeres i Teams administrasjonssenter ennå (disse er merket "kommer snart" i dokumentasjonen). I dette tilfellet, eller hvis du får en feil som "Vi kan ikke oppdatere policyen akkurat nå, men prøv det på nytt senere" i administrasjonssenteret for Microsoft Teams, anbefaler vi at du bruker PowerShell til å opprette eller endre teams møtepolicyer. 

Hvis du vil ha mer informasjon om møtepolicyer, kan du se følgende ressurser:

- Hvis du vil vite mer om hvordan du oppretter policyer, gjør endringer og tilordner brukere til policyen, kan du se [Administrere møtepolicyer i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Hvis du vil gjøre endringer i retningslinjene ved hjelp av PowerShell-cmdleter, kan du se [Teams PowerShell-oversikt](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Du må bruke [Skype for Business PowerShell-modulen](https://www.microsoft.com/download/details.aspx?id=39366) for teams-møtepolicyer. 
    - Se gjennom [cmdleterdokumentasjonen *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) hvis du vil ha mer informasjon.

