---
title: Bruke Giphy i Teams-samtaler
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
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982503"
---
# <a name="using-giphys-in-teams-conversations"></a>Bruke Giphy i Teams-samtaler

Giphy tilgang i Teams chat er aktivert som standard. Som administrator kan du kontrollere om Giphy er tilgjengelig for brukere ved [å angi en meldings policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) og sørge for at **Bruk giphy i samtaler** er **aktivert**.

Hvis GIF-en ikke fungerer som forventet i Teams-samtaler, må du bekrefte:

[Meldings policyen](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) må tillate giphy. Slik kontrollerer du ved å bruke PowerShell-cmdleter:

- Kontroller at du kan [administrere Teams med PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Kjør PowerShell-kommandoen [Get-CsTeamsMessagingPolicy-Identity global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) , og kontroller at **AllowGiphy** er satt til **True**.
- Hvis **AllowGiphy** er satt til **False** , kjører du følgende PowerShell-kommando [Sett-CsTeamsMessagingPolicy-Identity global-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Valg frie tilkoblede opplevelser](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) må være aktivert for å tillate tilgang til Giphy-URL-adressen.

> [!NOTE]
> Hvis du har flere Teams meldings policyer konfigurert for leieren din, kan du bestemme identiteten til policyen som er tilordnet den berørte brukeren med PowerShell-kommandoen [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Velg TeamsMessagingPolicy.
