---
title: Oppsett av DKIM i Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765275"
---
# <a name="setup-dkim-in-office-365"></a>Oppsett av DKIM i Office 365

Fullstendige instruksjoner for konfigurering av DKIM for egendefinerte domener i Office 365 er [her](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. For **hvert** egendefinert domene må du opprette **to** DKIM CNAME-postene på din domenets DNS-vertstjeneste (vanligvis domeneregistrar). Hvis du for eksempel contoso.com og fourthcoffee.com krever fire DKIM CNAME-poster: to for contoso.com og to for fourthcoffee.com.

   DKIM CNAME-postene for **hvert** egendefinert domene bruker følgende formater:

   - **Vertsnavn**:`selector1._domainkey.<CustomDomain>`

     **Peker til adressen eller verdi**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Vertsnavn**:`selector2._domainkey.<CustomDomain>`

     **Peker til adressen eller verdi**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> er teksten til venstre for `.mail.protection.outlook.com` i den tilpassede MX-posten for det egendefinerte domenet (for eksempel `contoso-com` for domenet contoso.com). \<InitialDomain\> er domenet du brukte da du registrerte deg for Office 365 (for eksempel contoso.onmicrosoft.com).

2. Når du har opprettet CNAME-postene for tilpasset domene, fullfører du fremgangsmåten nedenfor:

   en. [Logg på Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med jobbkonto eller skolekonto.

   b. Velg ikonet til startprogrammet for apper øverst til venstre, og velg **Administrator**.

   c. Utvid **Admin** i den nedre, venstre navigasjonen og velge **Exchange**.

   d. Gå til **beskyttelse mot** > **DKIM**.

   e. Velg domenet, og velg deretter **Aktiver** for **Logg meldinger for dette domenet med DKIM-signaturer**. Gjenta dette trinnet for hvert egendefinert domene.
