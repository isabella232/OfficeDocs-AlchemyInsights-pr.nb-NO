---
title: Skjule eller fjerne skjuling av Office 365-grupper eller -team fra adresselisten
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
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811465"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Skjule eller fjerne skjuling av Office 365-grupper eller -team fra adresselisten

Bruk følgende EXO PowerShell-kommando til å skjule eller fjerne skjuling av Office 365-gruppe/team fra adresselister (GAL) for Exchange-klienter (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Bruk følgende EXO PowerShell-kommando til å skjule eller fjerne skjuling av Office365-gruppen/teamene fra Exchange-klienter (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Hvis du vil ha detaljerte instruksjoner, kan du se [Skjule Office 365-grupper fra GAL- og Exchange-klienter](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
