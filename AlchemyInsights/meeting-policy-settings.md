---
title: Innstillinger for møte policy
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627583"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Administrere møte policyer i Microsoft Teams

Møte policyer brukes til å kontrollere funksjonene som er tilgjengelige for møtedeltakere for møter som planlegges av brukere i organisasjonen. Det kan hende at enkelte funksjoner i møte policyer ikke implementeres i Teams Administrasjonssenter ennå (disse kalles «kommer snart» i dokumentasjonen). I dette tilfellet, eller hvis du får en feilmelding som "vi kan ikke oppdatere policyen akkurat nå, men prøv igjen senere" i administrasjonssenteret for Microsoft Teams, anbefaler vi at du bruker PowerShell til å opprette eller endre møte policyer for Teams. 

Hvis du vil ha mer informasjon om møte policyer, kan du se følgende ressurser:

- Hvis du vil lære om hvordan du oppretter policyer, gjør endringer og tilordner brukere til policyen, kan du se [administrere møte policyer i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Hvis du vil gjøre policyendringer ved hjelp av PowerShell-cmdleter, kan du se [Teams PowerShell oversikt](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Du må bruke [Skype for Business PowerShell-modul](https://www.microsoft.com/download/details.aspx?id=39366) for Teams møte policyer. 
    - Se [dokumentasjonen *-CsTeamsMeetingPolicy cmdlets](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) hvis du vil ha mer informasjon.

**Merk:** Det kan ta opptil 24 timer for policyendringer trer i kraft for brukerne. Det er ikke sikkert du kan gjøre endringer i nylig opprettede policyer umiddelbart. vente i 4 timer og forsøke å endre en nyopprettet policy på nytt. Hvis du fortsatt har problemer, kan du prøve PowerShell.  