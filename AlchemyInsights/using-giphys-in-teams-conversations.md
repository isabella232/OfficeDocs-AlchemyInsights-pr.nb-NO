---
title: Bruke Giphys i Teams samtaler
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323529"
---
# <a name="using-giphys-in-teams-conversations"></a>Bruke Giphys i Teams samtaler

Giphys-tilgang i Teams er aktivert som standard. Som administrator kan du kontrollere om Giphys [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) er tilgjengelig for brukere ved å angi en meldingspolicy og sørge for at Bruk **Giphys** i samtaler er **På**.

Hvis GIF-filer ikke fungerer som forventet i Teams samtaler, kontrollerer du:

[Meldingspolicyen](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) må tillate Giphys. Slik bekrefter du ved hjelp av PowerShell-cmdleter:

- Kontroller at du kan [administrere Teams med PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Kjør PowerShell-kommandoen [Get-CsTeamsMessagingPolicy -Identity Global,](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) og kontroller at **AllowGiphy** er satt til **TRUE**.
- Hvis **AllowGiphy er** satt til **USANN,** kjører du følgende PowerShell-kommando [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Valgfrie tilkoblede](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) opplevelser må være aktivert for å gi tilgang til Giphy-nettadressen.

**Obs!** Hvis du har flere Teams-meldingspolicyer som er konfigurert for leieren, kan du bestemme identiteten til policyen som er tilordnet til den berørte brukeren med [PowerShell-kommandoen Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Velg TeamsMessagingPolicy.
