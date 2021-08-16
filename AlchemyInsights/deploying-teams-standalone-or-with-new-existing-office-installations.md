---
title: Distribuere Teams frittstående eller med nye eller eksisterende Office installasjoner
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
ms.openlocfilehash: e8baefafc1c2f9583345779c5ae7a9d3d0e05c4b3b7e1b3a74a9a22f7ceed02a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102211"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Distribuere Teams frittstående eller med nye eller eksisterende Office installasjoner

Microsoft Teams er nå inkludert som  en del av nye installasjoner av Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business og Office for Mac. Hvis du vil ha mer informasjon, [kan du se Når Microsoft Teams bli inkludert i nye installasjoner av Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Fra og med versjon 1906 i gjeldende kanal legges  Teams til i eksisterende installasjoner av Microsoft 365 Apps for enterprise (og Microsoft 365 Apps for business) på enheter som kjører Windows når du oppdaterer den eksisterende installasjonen til den nyeste versjonen. Hvis du vil ha mer informasjon, kan du se Hva [med eksisterende installasjoner av Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Hvis du ikke vil vente på denne utrullingsplanen, kan du distribuere [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) Teams som frittstående for brukerne ved å følge disse instruksjonene, eller du kan få brukerne til å installere Teams for seg selv fra [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Hvis organisasjonen ikke er klar til å distribuere Teams, har vi fremgangsmåten du kan [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) gjøre [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) for å ekskludere Teams fra nye eller eksisterende installasjoner av Office.  Hvis du vil Teams skal installeres, men ikke vil at Teams skal starte automatisk for brukeren etter at den er installert, kan du se Hindre at Microsoft Teams starter automatisk etter [installasjonen.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

Hvis ***du vil Teams*** fra en enhet som kjører Windows, kan du se [Avinstallere Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Hvis du vil Microsoft Teams fra flere målmaskiner eller brukere, [kan du se Microsoft Teams distribusjonsopprydding](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Hvis du bruker delte datamaskiner, Remote Desktop Services (RDS) eller Virtual Desktop Infrastructure (VDI), kan du se Delte datamaskin- og [VDI-miljøer med Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Hvis du bruker Office for Mac, kan du [Microsoft Teams installasjoner på en Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Når Teams er installert, oppdateres [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) den automatisk omtrent annenhver uke med nye funksjoner og kvalitetsoppdateringer. 