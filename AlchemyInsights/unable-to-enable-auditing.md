---
title: 2419-unable-to-enable-auditing
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
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007799"
---
# <a name="unable-to-enable-unified-auditing"></a>Kan ikke aktivere enhetlig overvåking

Når du prøver å aktivere enhetlig overvåking for organisasjonen, kan du få en feilmelding som ligner på følgende:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Følg disse trinnene for å løse dette problemet:

1. [Koble til å Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

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

- [Koble til å Exchange Online PowerShell ved hjelp av godkjenning med flere faktorer](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Aktivere eller deaktivere søk i overvåkingsloggen](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
