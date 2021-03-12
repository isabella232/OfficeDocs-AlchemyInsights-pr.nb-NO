---
title: Konfigurere DKIM med egendefinerte domener
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747642"
---
# <a name="set-up-dkim-with-custom-domains"></a>Konfigurere DKIM med egendefinerte domener

Du må publisere to CNAME-poster for hvert egendefinerte domene i DNS. Dette gjør du ved å bruke følgende format:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** er teksten til venstre for **.mail.protection.outlook.com** i den tilpassede MX-posten for det egendefinerte domenet (for eksempel contoso-com for domenet **contoso.com**). **InitialDomain** er domenet du brukte da du registrerte deg for Office 365 (for **eksempel contoso.onmicrosoft.com**).

Hvis du vil ha mer informasjon om DNS-poster, kan du se [Opprette DNS-poster hos en DNS-vertsleverandør for Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)