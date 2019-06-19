---
title: 2419--til-enable-overvåking
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065677"
---
# <a name="unable-to-enable-unified-auditing"></a>Kan ikke aktivere unified overvåking

Når du prøver å aktivere unified overvåking for Office 365-organisasjon, kan du få en feil som ligner følgende:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Hvis du vil løse dette problemet, gjør du følgende:

1. [Koble til Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Kjøre cmdleten følgende:

   ```
   Enable-OrganizationCustomization
   ```

3. Vent i 60 minutter for den forrige innstillingen skal tre i kraft.

4. Kjør følgende kommando i Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Hvis du vil ha mer informasjon, kan du se følgende artikler:

- [Koble til Exchange Online PowerShell ved hjelp av multifaktorautentisering](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Aktiver eller deaktiverer du Office 365 Overvåk Logg Søk](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
