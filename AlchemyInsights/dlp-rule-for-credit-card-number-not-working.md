---
title: DLP-regel for kreditt kort nummer fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679450"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-problemer med kreditt kort numre

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

**DLP-problemer med kreditt kort numre**

Har du problemer med **tap av datatap (DLP)** fungerer ikke for innhold som inneholder et **kreditt kort nummer** når du bruker en DLP sensitiv informasjons type i O365? Hvis dette er tilfelle, må du sørge for at innholdet inneholder den nødvendige informasjonen for å utløse DLP-policyen når den evalueres. For en **kreditt kort policy** konfigurert med et visshets nivå på 85%, evalueres for eksempel følgende, og må oppdages for at regelen skal utløse:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 sifre som kan formateres eller uformatert (dddddddddddddddd) og må bestå Luhn-testen.

- **[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Svært komplekst og robust mønster som oppdager kort fra alle hoved merker verden over, inkludert Visa, MasterCard, Discover Card, JCB, American Express, gave kort og Diner-kort.

- **[Kontroll sum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ja, Luhn-sjekksum

- **[Definisjon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** En DLP-policy er 85% sikker på at den har funnet denne typen sensitiv informasjon hvis, innenfor en nærhet av 300-tegn:

  - Funksjonen Func_credit_card finner innhold som Sams varer med mønsteret.

  - Ett av følgende er sant:

  - Et nøkkel ord fra Keyword_cc_verification blir funnet.

  - Et nøkkel ord fra Keyword_cc_name blir funnet

  - Funksjonen Func_expiration_date finner en dato i riktig dato format.

  - Kontroll sum trinnene

    Følgende eksempel vil for eksempel utløse en policy for et DLP-kreditt kort nummer:

  - Visa: 4485 3647 3952 7352
  
  - Utløper: 2/2009

Hvis du vil ha mer informasjon om hva som kreves for at et **kreditt kort nummer** skal registreres for innholdet, kan du se følgende del i denne artikkelen: [hva de sensitive informasjons typene ser ut for kreditt kort #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Hvis du bruker en annen innebygd sensitiv informasjons type, kan du se følgende artikkel for informasjon om hva som er nødvendig for andre typer: [hva de sensitive informasjons typene ser etter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  