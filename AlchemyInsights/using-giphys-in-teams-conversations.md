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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104317"
---
# <a name="using-giphys-in-teams-conversations"></a>Bruke Giphys i Teams samtaler

Giphys-tilgang i Teams chat er aktivert som standard. Som administrator kan du kontrollere om Giphys [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) er tilgjengelig for brukere ved å angi en meldingspolicy og sørge for at Bruk **Giphys** i samtaler er **På**.

Hvis GIF-filer ikke fungerer som forventet i Teams samtaler, kontrollerer du:

[Meldingspolicyen](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) må tillate Giphys. Slik bekrefter du ved hjelp av PowerShell-cmdleter:

- Kontroller at du kan [administrere Teams med PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Kjør PowerShell-kommandoen [Get-CsTeamsMessagingPolicy -Identity Global,](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) og kontroller at **AllowGiphy** er satt til **TRUE**.
- Hvis **AllowGiphy er** satt til **USANN,** kjører du følgende PowerShell-kommando [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Valgfrie tilkoblede](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) opplevelser må være aktivert for å gi tilgang til Giphy-nettadressen.

> [!NOTE]
> Hvis du har flere Teams-meldingspolicyer som er konfigurert for leieren, kan du bestemme identiteten til policyen som er tilordnet til den berørte brukeren med [PowerShell-kommandoen Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Velg TeamsMessagingPolicy.
