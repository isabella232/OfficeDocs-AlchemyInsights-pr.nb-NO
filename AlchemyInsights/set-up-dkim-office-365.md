---
title: Oppsett DKIM i Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666273"
---
# <a name="setup-dkim-in-office-365"></a>Oppsett DKIM i Office 365

De fullstendige instruksjonene for konfigurering av DKIM for egendefinerte domener i Office 365 er [her](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. For **hvert** egendefinerte domene må du opprette **to** DKIM CNAME Records på domenets DNS-vertstjenesten (vanligvis domeneregistratoren). Contoso.com og fourthcoffee.com krever for eksempel fire DKIM CNAME-poster: to for contoso.com og to for fourthcoffee.com.

   DKIM CNAME-postene for **hvert** egendefinerte domene bruker følgende formater:

   - **Vertsnavn**:`selector1._domainkey.<CustomDomain>`

     **Peker til adresse eller verdi**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Vertsnavn**:`selector2._domainkey.<CustomDomain>`

     **Peker til adresse eller verdi**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> er teksten til venstre for `.mail.protection.outlook.com` i den tilpassede MX-posten for det egendefinerte domenet (for eksempel `contoso-com` for domenet contoso.com). \<InitialDomain\> er domenet du brukte da du registrerte deg for Office 365 (for eksempel contoso.onmicrosoft.com).

2. Når du har opprettet CNAME-postene for de egendefinerte domenene, fullfører du følgende instruksjoner:

   A. [Logg på Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med jobbkonto eller skolekonto.

   B. Velg ikonet til startprogrammet for apper øverst til venstre, og velg **Administrator**.

   C. Utvid **administrator** i nedre venstre navigasjon, og velg **Exchange**.

   D. Gå til **Protection** > **DKIM**.

   E. Velg domenet, og velg deretter **Aktiver** for **Sign-meldinger for dette domenet med DKIM-signaturer**. Gjenta dette trinnet for hvert egendefinerte domene.
