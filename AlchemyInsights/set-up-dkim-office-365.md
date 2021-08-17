---
title: Konfigurere DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108565"
---
# <a name="setup-dkim"></a>Konfigurere DKIM

De fullstendige instruksjonene for å konfigurere DKIM for egendefinerte domener i Microsoft 365 [her](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. For **hvert** egendefinerte domene må du opprette to **DKIM** CNAME-poster på domenets DNS-vertstjeneste (vanligvis domeneregistratoren). Du kan for eksempel contoso.com og fourthcoffee.com fire DKIM CNAME-poster: to for contoso.com og to for fourthcoffee.com.

   DKIM CNAME-postene for **hvert** egendefinerte domene bruker følgende formater:

   - **Vertsnavn:**`selector1._domainkey.<CustomDomain>`

     **Peker til adresse eller verdi:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Vertsnavn:**`selector2._domainkey.<CustomDomain>`

     **Peker til adresse eller verdi:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> er teksten til venstre for i den tilpassede MX-posten for det egendefinerte domenet (for eksempel `.mail.protection.outlook.com` `contoso-com` for domenet contoso.com). \<InitialDomain\>er domenet du brukte da du registrerte deg for Microsoft 365 (for eksempel contoso.onmicrosoft.com).

2. Når du har opprettet CNAME-postene for de egendefinerte domenene, følger du disse instruksjonene:

   a. [logg på Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med jobb- eller skolekontoen.

   b. Velg ikonet til startprogrammet for apper øverst til venstre, og velg **Administrator**.

   c. Utvid Administrator nederst til **venstre,** og velg **Exchange**.

   d. Gå til **Beskyttelse**  >  **DKIM**.

   e. Velg domenet, og velg deretter **Aktiver** for **Signer meldinger for dette domenet med DKIM-signaturer**. Gjenta dette trinnet for hvert egendefinerte domene.
