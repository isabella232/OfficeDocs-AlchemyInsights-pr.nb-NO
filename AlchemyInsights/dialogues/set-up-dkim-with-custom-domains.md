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
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525414"
---
# <a name="set-up-dkim-with-custom-domains"></a><span data-ttu-id="6e03a-102">Konfigurere DKIM med egendefinerte domener</span><span class="sxs-lookup"><span data-stu-id="6e03a-102">Set up DKIM with custom domains</span></span>

<span data-ttu-id="6e03a-103">Du må publisere to CNAME-poster for hvert egendefinerte domene i DNS.</span><span class="sxs-lookup"><span data-stu-id="6e03a-103">You must publish two CNAME records for each custom domain in DNS.</span></span> <span data-ttu-id="6e03a-104">Dette gjør du ved å bruke følgende format:</span><span class="sxs-lookup"><span data-stu-id="6e03a-104">To do this, use the following format:</span></span>

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> <span data-ttu-id="6e03a-105">**DomainGUID** er teksten til venstre for **.mail.protection.outlook.com** i den tilpassede MX-posten for det egendefinerte domenet (for eksempel contoso-com for domenet **contoso.com).**</span><span class="sxs-lookup"><span data-stu-id="6e03a-105">**DomainGUID** is the text to the left of **.mail.protection.outlook.com** in the customized MX record for the custom domain (for example, contoso-com for the domain **contoso.com**).</span></span> <span data-ttu-id="6e03a-106">**InitialDomain** er domenet du brukte da du registrerte deg for Office 365 (for eksempel **contoso.onmicrosoft.com).**</span><span class="sxs-lookup"><span data-stu-id="6e03a-106">**InitialDomain** is the domain you used when you signed up for Office 365 (for example, **contoso.onmicrosoft.com**).</span></span>

<span data-ttu-id="6e03a-107">Hvis du vil ha mer informasjon om DNS-poster, kan du se [Opprette DNS-poster hos en DNS-vert for Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)</span><span class="sxs-lookup"><span data-stu-id="6e03a-107">For more information about DNS records, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>