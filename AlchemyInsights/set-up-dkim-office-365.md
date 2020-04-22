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
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645681"
---
# <a name="setup-dkim"></a>Oppsett DKIM

De fullstendige instruksjonene for å konfigurere DKIM for egendefinerte domener i Microsoft 365 er [her](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. For **hvert** egendefinerte domene må du opprette **to** DKIM CNAME-poster på domenets DNS-vertstjeneste (vanligvis domeneregistratoren). Contoso.com og fourthcoffee.com krever for eksempel fire DKIM CNAME-poster: to for contoso.com og to for fourthcoffee.com.

   DKIM CNAME-postene for **hvert** egendefinerte domene bruker følgende formater:

   - **Vertsnavn**:`selector1._domainkey.<CustomDomain>`

     **Peker til adresse eller verdi**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Vertsnavn**:`selector2._domainkey.<CustomDomain>`

     **Peker til adresse eller verdi**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> er teksten til `.mail.protection.outlook.com` venstre for i den tilpassede MX-posten `contoso-com` for det egendefinerte domenet (for eksempel for domenet contoso.com). \<InitialDomain\> er domenet du brukte da du registrerte deg for Microsoft 365 (for eksempel contoso.onmicrosoft.com).

2. Når du har opprettet CNAME-postene for de egendefinerte domenene, gjør du følgende:

   A. [logg på Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med jobb- eller skolekontoen.

   B. Velg ikonet til startprogrammet for apper øverst til venstre, og velg **Administrator**.

   C. Utvid **Administrator** i navigasjonen nederst til venstre, og velg **Exchange**.

   D. Gå til **Beskyttelse** > **DKIM**.

   E. Velg domenet, og velg deretter **Aktiver** for **Sign-meldinger for dette domenet med DKIM-signaturer**. Gjenta dette trinnet for hvert egendefinerte domene.
