---
title: 2419 – kan ikke aktivere overvåking
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767608"
---
# <a name="unable-to-enable-unified-auditing"></a>Kan ikke aktivere enhetlig overvåking

Når du prøver å aktivere enhetlig overvåking for organisasjonen, kan det hende du får en feil melding som ligner på følgende:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Følg denne Fremgangs måten for å løse dette problemet:

1. [Koble til Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Kjør følgende cmdlet:

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

-  [Aktivere eller deaktivere søk i overvåkings loggen](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
