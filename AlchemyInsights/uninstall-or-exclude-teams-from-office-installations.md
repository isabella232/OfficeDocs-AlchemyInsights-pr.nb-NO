---
title: Avinstallere eller ekskludere Teams fra Office-installasjoner
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
- "2662"
- "9000660"
ms.openlocfilehash: 22d69db749671afdfe7a809d1bc598e2ad1891d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658230"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Avinstallere eller ekskludere Teams fra nye eller eksisterende Office-installasjoner

Microsoft Teams er inkludert som en del av Microsoft 365-apper for Enterprise, Microsoft 365-apper for Business og Office for Mac.

- Bruk [distribusjons verktøyet for Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) til å utelate Teams fra nye installasjoner av Office.
- Hvis du vil *avinstallere* Teams fra en enhet som kjører Windows, kan du se [avinstallere Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Hvis du vil rydde opp i Microsoft Teams fra flere mål maskiner eller brukere, kan du se [rydde opp i Microsoft Teams-distribusjon](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- Bruk [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) -alternativet for å hindre at Microsoft Teams installeres automatisk med Office.
- Bruk [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) -alternativet, *før Teams er installert*, for å hindre at Microsoft Teams starter automatisk etter installasjon.

Hvis du bruker Office for Mac, kan du se [Microsoft Teams-installasjoner på en Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).