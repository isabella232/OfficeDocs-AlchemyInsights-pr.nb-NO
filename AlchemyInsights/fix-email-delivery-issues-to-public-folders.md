---
title: Løse problemer med levering av e-post til e-postaktiverte fellesmapper
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
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068821"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Løse problemer med levering av e-post til e-postaktiverte fellesmapper

Hvis eksterne avsendere ikke kan sende meldinger til e-postaktiverte fellesmapper, og avsenderne får feilmeldingen: Finner ikke **(550 5.4.1),** kontrollerer du at e-postdomenet for fellesmappen er konfigurert som et internt reledomene i stedet for et autoritativt domene:

1. Åpne Exchange [(EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Gå til **E-postflyt** \> **Godtatte domener,** velg det godtatte domenet, og klikk deretter **Rediger**.

3. Hvis domenetypen er satt til **Autoritativ** på egenskapssiden som åpnes, endrer du verdien til Intern **videresending,** og deretter klikker du **Lagre**.

Hvis eksterne avsendere får feilen du ikke har tillatelse **til (550 5.7.13),** kjører du følgende kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) for å se tillatelsene for anonyme brukere i fellesmappen:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For eksempel `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Hvis du vil tillate eksterne brukere å sende e-post til denne fellesmappen, legger du til CreateItems-tilgang direkte til brukeren Anonym. For eksempel `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
