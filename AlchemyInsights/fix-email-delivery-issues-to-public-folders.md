---
title: Løse problemer med levering av e-post til e-postaktiverte felles mapper
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366473"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Løse problemer med levering av e-post til e-postaktiverte felles mapper

Hvis eksterne avsendere ikke kan sende meldinger til de e-postaktiverte felles mappene, og avsenderne får feil meldingen: **ble ikke funnet (550 5.4.1)**, må du kontrollere at e-postdomenene for felles mappen er konfigurert som et internt Relay-domene i stedet for et autoritativt domene:

1. Åpne [administrasjons senteret for Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Gå til **e-postflyt** \> **godkjente domener**, Velg godkjent domene, og klikk deretter **Rediger**.

3. På Egenskaper-siden som åpnes, hvis domene typen er satt til **autoritativ**, endrer du verdien til **intern videre sending** og klikker deretter **Lagre**.

Hvis eksterne avsendere får feilen **du ikke har tilgang til (550 5.7.13)**, kjører du følgende kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) for å se tillatelsene for anonyme brukere i felles mappen:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For eksempel `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Hvis du vil tillate at eksterne brukere sender e-post til denne felles mappen, kan du legge til CreateItems Access-tilgang direkte i den anonyme brukeren. For eksempel `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
