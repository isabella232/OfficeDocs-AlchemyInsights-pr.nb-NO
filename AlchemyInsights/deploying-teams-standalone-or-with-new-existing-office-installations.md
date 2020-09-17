---
title: Distribuere Teams som fritt stående eller med nye eller eksisterende Office-installasjoner
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806768"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Distribuere Teams som fritt stående eller med nye eller eksisterende Office-installasjoner

Microsoft Teams er nå inkludert som en del av ***nye installasjoner*** av Microsoft 365-apper for Enterprise, Microsoft 365-apper for bedrifter og Office for Mac. Hvis du vil ha mer informasjon, kan du se [når vil Microsoft Teams begynne å være inkludert i nye installasjoner av Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

I tillegg, som starter med versjon 1906 i gjeldende kanal, blir Teamne ***lagt til i eksisterende installasjoner*** av Microsoft 365-apper for Enterprise (og Microsoft 365-apper for bedrifter) på enheter som kjører Windows når du oppdaterer den eksisterende installasjonen til den nyeste versjonen. Hvis du vil ha mer informasjon, kan du se [Hva med eksisterende installasjoner av Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Hvis du ikke vil vente på denne planleggings planen, kan du distribuere Teams som fritt stående for brukerne ved å [følge disse instruksjonene](https://docs.microsoft.com/MicrosoftTeams/msi-deployment),   eller du kan få brukerne til å installere Teams for seg selv  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Hvis organisasjonen ikke er klar til å distribuere team, har vi trinnene du kan gjøre for å ***utelate team*** fra [nye](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) eller [eksisterende](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installasjoner av Office. Hvis du vil at team skal installeres, men ikke vil at Teams skal starte automatisk for brukeren etter at de er installert, kan du se [forhindre at Microsoft Teams starter automatisk etter installasjon](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Hvis du vil ***avinstallere Teams*** fra en enhet som kjører Windows, kan du se [avinstallere Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Hvis du vil rydde opp i Microsoft Teams fra flere mål maskiner eller brukere, kan du se [fjerne Microsoft Teams-distribusjon](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Hvis du bruker delte data maskiner, RDS (Remote Desktop Services) eller Virtual Desktop-infrastruktur (VDI), kan du se [delt data maskin-og VDI-miljøer med Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Hvis du bruker Office for Mac, kan du se [Microsoft Teams-installasjoner på en Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Etter at Teams er installert, [oppdateres den automatisk](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) omtrent hver annen uke med nye funksjoner og kvalitets oppdateringer. 