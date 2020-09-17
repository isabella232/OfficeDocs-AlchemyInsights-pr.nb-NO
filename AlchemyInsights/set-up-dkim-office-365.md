---
title: Oppsett-DKIM
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
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808716"
---
# <a name="setup-dkim"></a>Oppsett-DKIM

De fullstendige instruksjonene for å konfigurere DKIM for egen definerte domener i Microsoft 365 er [her](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. For **hvert** egen definert domene må du opprette **to** DKIM CNAME-poster hos DNS-verten for domenet (vanligvis domene registreren). Contoso.com og fourthcoffee.com krever for eksempel fire DKIM CNAME-poster: to for contoso.com og to for fourthcoffee.com.

   DKIM CNAME-poster for **hvert** egen definert domene bruker følgende formater:

   - **Verts navn**: `selector1._domainkey.<CustomDomain>`

     **Peker til adresse eller verdi**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Verts navn**: `selector2._domainkey.<CustomDomain>`

     **Peker til adresse eller verdi**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> er teksten til venstre for den `.mail.protection.outlook.com` tilpassede MX-posten for det egen definerte domenet (for eksempel `contoso-com` for domenet contoso.com). \<InitialDomain\> er domenet du brukte da du registrerte deg for Microsoft 365 (for eksempel contoso.onmicrosoft.com).

2. Når du har opprettet CNAME-postene for de egen definerte domenene, må du fullføre følgende instruksjoner:

   a. [Logg på Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med jobb-eller skole kontoen.

   b. Velg ikonet til startprogrammet for apper øverst til venstre, og velg **Administrator**.

   c. Utvid **administrator** i nedre venstre navigasjon, og velg **Exchange**.

   d. Gå til **beskyttelses**  >  **DKIM**.

   e. Velg domenet, og velg deretter **Aktiver** for **signerings meldinger for dette domenet med DKIM-signaturer**. Gjenta dette trinnet for hvert egen definert domene.
