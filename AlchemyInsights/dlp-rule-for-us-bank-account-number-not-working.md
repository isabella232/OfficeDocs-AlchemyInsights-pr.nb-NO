---
title: DLP-regel for amerikansk bank konto nummer fungerer ikke
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679305"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-problemer med amerikanske bank konto numre

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

**DLP-problemer med amerikanske bank konto numre**

Har du problemer med **tap av datatap (DLP)** fungerer ikke for innhold som inneholder et **amerikansk bank konto nummer** når du bruker en DLP sensitiv informasjons type i O365? Hvis det er tilfelle, må du kontrollere at innholdet inneholder den nødvendige informasjonen for hva DLP-policyen ser ut når den evalueres.
  
For en **amerikansk bank konto nummer** policy, som for eksempel er konfigurert med et konfidenskoeffisienten-nivå på 85%, evalueres følgende og må oppdages for at regelen skal utløse:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 sifre

- **[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 påfølgende sifre.

- **[Kontroll sum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nei, det er ingen kontroll sum

- **[Definisjon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** En DLP-policy er 75% sikker på at den har funnet denne typen sensitiv informasjon hvis, innenfor en nærhet av 300-tegn:

  - Det vanlige uttrykket Regex_usa_bank_account_number finner innhold som Sams varer med mønsteret

  - Et nøkkel ord fra Keyword_usa_Bank_Account blir funnet.

    Følgende eksempel vil for eksempel utløse den **amerikanske bank konto nummer** policyen: kontrollere konto 78344011

Hvis du vil ha mer informasjon om hva som kreves for at et **amerikansk bank konto nummer** skal oppdages for innholdet, kan du se følgende avsnitt i denne artikkelen: [hva de sensitive informasjons typene ser ut for amerikansk bank konto nummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Hvis du bruker en annen innebygd sensitiv informasjons type, kan du se følgende artikkel for informasjon om hva som er nødvendig for andre typer: [hva de sensitive informasjons typene ser etter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  