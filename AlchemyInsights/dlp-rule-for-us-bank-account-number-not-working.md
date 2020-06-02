---
title: DLP-regel for amerikansk bankkontonummer fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507343"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-problemer med amerikanske bankkontonumre

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

**DLP-problemer med amerikanske bankkontonumre**

Har du problemer med **at Data Loss Prevention (DLP)** ikke fungerer for innhold som inneholder et amerikansk **bankkontonummer** når du bruker en DLP-sensitiv informasjonstype i O365? I så fall må du kontrollere at innholdet inneholder den nødvendige informasjonen for hva DLP-policyen ser etter når det evalueres.
  
For en policy for **amerikansk bankkontonummer** som er konfigurert med et konfidensnivå på 85 %, evalueres følgende og må oppdages for at regelen skal utløses:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 sifre

- **[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 sifre på rad.

- **[Sjekksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nei, det er ingen kontrollsum

- **[Definisjon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** En DLP-policy er 75 % sikker på at den oppdages denne typen sensitiv informasjon hvis, i nærheten av 300 tegn:

  - Det regulære uttrykket Regex_usa_bank_account_number finner innhold som samsvarer med mønsteret

  - Du finner et nøkkelord fra Keyword_usa_Bank_Account.

    Følgende eksempel utløses for eksempel for policyen **for us bankkontonummer:** Kontrollere konto 78344011

Hvis du vil ha mer informasjon om hva som kreves for at et **amerikansk bankkontonummer** skal oppdages for innholdet ditt, kan du se følgende del i denne artikkelen: [Hva sensitive informasjonstyper ser etter amerikansk bankkontonummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Hvis du bruker en annen innebygd sensitiv informasjonstype, kan du se følgende artikkel for informasjon om hva som kreves for andre typer: [Hva sensitive informasjonstyper ser etter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  