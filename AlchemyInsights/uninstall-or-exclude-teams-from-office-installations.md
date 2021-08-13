---
title: Avinstallere eller utelate Teams fra Office installasjoner
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
- "2662"
- "9000660"
ms.openlocfilehash: a960c96abf6215e3a34908ce8669a0c61298daac829343b3673dbfef0c4cbfc7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007727"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Avinstallere eller utelate Teams fra nye eller eksisterende Office installasjoner

Microsoft Teams er inkludert som en del av Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business og Office for Mac.

- Bruk [distribusjonsverktøyet Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) til å Teams fra nye installasjoner av Office.
- Hvis *du vil* Teams fra en enhet som kjører Windows, kan du se [Avinstallere Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Hvis du vil Microsoft Teams fra flere målmaskiner eller [brukere, kan du Microsoft Teams rydde opp i distribusjonen.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)
- Bruk [alternativet PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) for å hindre Microsoft Teams å installere automatisk med Office.
- Bruk [preventFirstLaunchAfterInstall-alternativet](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *før* Teams er installert , for å hindre at Microsoft Teams starter automatisk etter installasjonen.

Hvis du bruker Office for Mac, kan du [Microsoft Teams installasjoner på en Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).