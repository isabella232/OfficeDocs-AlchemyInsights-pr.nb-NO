---
title: 2419-kan ikke-aktivere-revisjon
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510437"
---
# <a name="unable-to-enable-unified-auditing"></a>Kan ikke aktivere enhetlig sporing av endringer

Når du prøver å aktivere enhetlig sporing av endringer for organisasjonen, kan du få en feilmelding som ligner på følgende:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Hvis du vil løse dette problemet, gjør du følgende:

1. [Koble til Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Kjør cmdleten følgende:

   ```
   Enable-OrganizationCustomization
   ```

3. Vent i 60 minutter før den forrige innstillingen trer i kraft.

4. Kjør følgende kommando i Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Hvis du vil ha mer informasjon, kan du se følgende artikler:

- [Koble til Exchange Online PowerShell ved hjelp av godkjenning med flere faktorer](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Aktivere eller deaktivere søk i overvåkingsloggen](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
