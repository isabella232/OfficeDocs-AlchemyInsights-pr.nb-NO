---
title: Løse problemer med e-postlevering til e-postaktiverte fellesmapper
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716361"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Løse problemer med e-postlevering til e-postaktiverte fellesmapper

Hvis eksterne avsendere ikke kan sende meldinger til de e-postaktiverte fellesmappene, og avsenderne får feilmeldingen: **Finner ikke feilen (550 5.4.1),** må du kontrollere at e-postdomenet for fellesmappen er konfigurert som et internt relédomene i stedet for et autoritativt domene:

1. Åpne [administrasjonssenteret for Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Gå til **E-postflyt** \> **Godtatt e-postdomener**, velg det godtatte domenet, og klikk deretter **Rediger**.

3. Hvis domenetypen er satt til **Autoritativ**på egenskapssiden som åpnes, endrer du verdien til **Intern relé** på egenskapssiden som åpnes, og deretter klikker du **Lagre**.

Hvis eksterne avsendere får feilmeldingen **du ikke har tillatelse (550 5.7.13),** kjører du følgende kommando i Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) for å se tillatelsene for anonyme brukere i fellesmappen:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`For eksempel `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`. .

Hvis du vil tillate eksterne brukere å sende e-post til denne fellesmappen, legger du til Rettigheten CreateItems-tilgang til brukeren Anonym. For eksempel `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`. .
