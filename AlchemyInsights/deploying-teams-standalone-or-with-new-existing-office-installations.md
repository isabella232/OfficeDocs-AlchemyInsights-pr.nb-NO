---
title: Distribuere teams som frittstående eller med nye eller eksisterende Office-installasjoner
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: ffa91eaf333792af149feda25f9a377ed591b597
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010227"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Distribuere teams som frittstående eller med nye eller eksisterende Office-installasjoner

Microsoft Teams er nå inkludert som en del av ***nye installasjoner*** av Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business og Office for Mac. Hvis du vil ha mer informasjon, kan du se [Når blir Microsoft Teams inkludert i nye installasjoner av Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

I tillegg, fra versjon 1906 i månedlig kanal, vil Teams bli ***lagt til eksisterende installasjoner*** av Microsoft 365 Apps for enterprise (og Microsoft 365 Apps for business) på enheter som kjører Windows når du oppdaterer den eksisterende installasjonen til den nyeste versjonen. Hvis du vil ha mer informasjon, kan du se [Hva med eksisterende installasjoner av Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Hvis du ikke vil vente på denne tidsplanen for samleoppdateringen, kan du distribuere Teams som frittstående for brukerne [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)ved å følge disse [instruksjonene,](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) eller du kan få brukerne til å installere Teams selv fra .

Hvis organisasjonen ikke er klar til å distribuere teams, har vi fremgangsmåten du kan utføre for å ***ekskludere teams*** fra [nye](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) eller [eksisterende](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installasjoner av Office. Hvis du vil at Teams skal installeres, men ikke vil at Teams skal starte automatisk for brukeren etter at den er installert, kan du se [Hindre at Microsoft Teams starter automatisk etter installasjonen](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Hvis du vil ***avinstallere Teams*** fra en enhet som kjører Windows, kan du se [Avinstallere Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Hvis du vil rydde opp i Microsoft Teams fra flere målmaskiner eller brukere, kan du se [Opprydding i Microsoft Teams-distribusjon](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Hvis du bruker delte datamaskiner, Remote Desktop Services (RDS) eller Virtual Desktop Infrastructure (VDI), kan du se [Delte datamaskin- og VDI-miljøer med Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Hvis du bruker Office for Mac, kan du se [Microsoft Teams-installasjoner på en Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Når Teams er installert, [oppdateres](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) den automatisk omtrent annenhver uke med nye funksjoner og kvalitetsoppdateringer. 