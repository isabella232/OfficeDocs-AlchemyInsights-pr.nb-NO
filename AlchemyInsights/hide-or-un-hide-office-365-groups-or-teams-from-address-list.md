---
title: Skjule eller fjerne Office 365 grupper eller team fra adresselisten
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088405"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Skjule eller fjerne Office 365 grupper eller team fra adresselisten

Bruk følgende EXO PowerShell-kommando til å skjule Office 365 gruppe/team fra adresselister (GAL) Exchange klienter (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Bruk følgende EXO PowerShell-kommando til å skjule eller fjerne skjuling av Office365-gruppen/teamene Exchange klienter (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Hvis du vil ha detaljerte [instruksjoner, kan du se Skjule Office 365 grupper fra gal](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)og Exchange klienter .
