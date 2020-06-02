---
title: Oppsett DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509393"
---
# <a name="setup-dkim"></a>Oppsett DKIM

De fullstendige instruksjonene for å konfigurere DKIM for egendefinerte domener i Microsoft 365 er [her](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. For **hvert** egendefinerte domene må du opprette **to** DKIM CNAME-poster på domenets DNS-vertstjeneste (vanligvis domeneregistratoren). contoso.com og fourthcoffee.com krever for eksempel fire DKIM CNAME-poster: to for contoso.com og to for fourthcoffee.com.

   DKIM CNAME-postene for **hvert** egendefinerte domene bruker følgende formater:

   - **Vertsnavn**:`selector1._domainkey.<CustomDomain>`

     **Peker til adresse eller verdi:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Vertsnavn**:`selector2._domainkey.<CustomDomain>`

     **Peker til adresse eller verdi:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>er teksten til venstre `.mail.protection.outlook.com` for i den tilpassede MX-posten for det egendefinerte domenet (for eksempel for domenet `contoso-com` contoso.com). \<InitialDomain\>er domenet du brukte da du registrerte deg for Microsoft 365 (for eksempel contoso.onmicrosoft.com).

2. Når du har opprettet CNAME-postene for de egendefinerte domenene, fullfører du følgende instruksjoner:

   a. [logg på Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med jobb- eller skolekontoen.

   b. Velg ikonet til startprogrammet for apper øverst til venstre, og velg **Administrator**.

   c. Utvid **Administrator** i navigasjonen nederst til venstre, og velg **Exchange**.

   D. Gå til **Beskyttelse**  >  **DKIM**.

   E. Velg domenet, og velg deretter **Aktiver** for **Signer-meldinger for dette domenet med DKIM-signaturer**. Gjenta dette trinnet for hvert egendefinerte domene.
