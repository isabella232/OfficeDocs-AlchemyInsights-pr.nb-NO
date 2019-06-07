---
title: Løse problemer for levering av e-post til e-post fellesmapper
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 900b6cc2765937ee005c7e7dce5d33bbdf582601
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752679"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Løse problemer for levering av e-post til e-post fellesmapper

Hvis eksterne avsendere ikke kan sende meldinger til din e-post fellesmapper og avsendere får feilmeldingen: **kunne ikke finne (550 5.4.1)**, kontroller e-domenet for fellesmappen er konfigurert som et domene for intern videresending i stedet for en autoritative domenet:

1. Åpne [administrasjonssenteret for Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Gå til **e-postflyt** \> **godkjente domener**, velg det godtatte domenet, og klikk deretter **Rediger**.

3. I egenskapene for siden som åpnes, hvis domenetypen er satt til **Authoritative**, endrer du verdien til **intern videresending** , og klikk deretter **Lagre**.

Hvis eksterne avsendere får feil **du ikke har tillatelse (550 5.7.13)**, kan du kjøre følgende kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) for å se hvilke tillatelser for anonyme brukere i fellesmappen:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`For eksempel `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Hvis du vil tillate at eksterne brukere å sende e-post til denne mappen, legge til CreateItems-access høyre bruker anonym. For eksempel `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
