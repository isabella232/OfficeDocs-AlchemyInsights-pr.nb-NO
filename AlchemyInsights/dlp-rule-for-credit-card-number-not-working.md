---
title: DLP-regel for kredittkortnummer fungerer ikke
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
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005099"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-problemer med kredittkortnumre

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

**DLP-problemer med kredittkortnumre**

Har du problemer med hindring av tap av data **(DLP)** fungerer ikke for innhold som inneholder et kredittkortnummer når du bruker en DLP-sensitiv informasjonstype i O365?  Hvis dette er det, må du kontrollere at innholdet inneholder den nødvendige informasjonen for å utløse DLP-policyen når den evalueres. For en kredittkortpolicy som er konfigurert med et konfidensnivå på 85 %, evalueres for eksempel følgende og må oppdages for at regelen skal utløse: 
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 sifre som kan formateres eller uformateres (ddddddddd) og må bestå Luhn-testen.

- **[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Svært komplekst og robust mønster som oppdager kort fra alle store merker over hele verden, inkludert Visa, MasterCard, Discover Card, JCB, American Express, gavekort og restaurantkort.

- **[Sjekksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ja, Luhn-sjekksummen

- **[Definisjon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** En DLP-policy er 85 % sikker på at den har oppdaget denne typen sensitiv informasjon hvis den er i nærheten av 300 tegn:

  - Funksjonen Func_credit_card finner innhold som samsvarer med mønsteret.

  - Ett av følgende er sant:

  - Et nøkkelord fra Keyword_cc_verification finnes.

  - Et nøkkelord fra Keyword_cc_name finnes

  - Funksjonen Func_expiration_date en dato i riktig datoformat.

  - Kontrollsummen passerer

    Følgende eksempel vil for eksempel utløse en policy for DLP-kredittkortnummer:

  - Visa: 4485 3647 3952 7352
  
  - Utløper: 02.02.2009

Hvis du vil ha mer  informasjon om hva som kreves for at et kredittkortnummer skal oppdages for innholdet ditt, kan du se følgende del i denne artikkelen: Hvilke typer sensitive opplysninger ser [etter kredittkort#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Hvis du bruker en annen innebygd sensitiv informasjonstype, kan du se følgende artikkel for informasjon om hva som kreves for andre typer: Hva de [sensitive informasjonstypene ser etter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  