---
title: DLP-regel for kredittkortnummer fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507415"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-problemer med kredittkortnumre

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

**DLP-problemer med kredittkortnumre**

Har du problemer med **at Data Loss Prevention (DLP)** ikke fungerer for innhold som inneholder et **kredittkortnummer** når du bruker en DLP-sensitiv informasjonstype i O365? I så fall må du kontrollere at innholdet inneholder den nødvendige informasjonen for å utløse DLP-policyen når den evalueres. For en **kredittkortpolicy** som er konfigurert med et konfidensnivå på 85 %, evalueres følgende og må oppdages for at regelen skal utløses:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 sifre som kan formateres eller uformatert (ddddddddddddddddddd) og må bestå Luhn-testen.

- **[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Svært komplekse og robuste mønster som oppdager kort fra alle store merker over hele verden, inkludert Visa, MasterCard, Discover Card, JCB, American Express, gavekort og dinerkort.

- **[Sjekksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ja, Luhn-kontrollsummen

- **[Definisjon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** En DLP-policy er 85 % sikker på at den oppdages denne typen sensitiv informasjon hvis, i nærheten av 300 tegn:

  - Funksjonen Func_credit_card finner innhold som samsvarer med mønsteret.

  - Ett av følgende er sant:

  - Du finner et nøkkelord fra Keyword_cc_verification.

  - Et nøkkelord fra Keyword_cc_name blir funnet

  - Funksjonen finner Func_expiration_date en dato i riktig datoformat.

  - Kontrollsummen passerer

    Følgende eksempel utløses for eksempel for en DLP-kredittkortnummerpolicy:

  - Visum: 4485 3647 3952 7352
  
  - Utløper: 2/2009

Hvis du vil ha mer informasjon om hva som kreves for at et **kredittkortnummer** skal oppdages for innholdet ditt, kan du se følgende del i denne artikkelen: [Hva sensitiv informasjonstyper ser etter kredittkort#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Hvis du bruker en annen innebygd sensitiv informasjonstype, kan du se følgende artikkel for informasjon om hva som kreves for andre typer: [Hva sensitive informasjonstyper ser etter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  