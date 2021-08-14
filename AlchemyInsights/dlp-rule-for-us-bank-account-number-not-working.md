---
title: DLP-regel for amerikansk bankkontonummer fungerer ikke
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
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005027"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-problemer med amerikanske bankkontonumre

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

**DLP-problemer med amerikanske bankkontonumre**

Har du problemer med hindring av datatap **(DLP)** som ikke fungerer for innhold som inneholder et amerikansk bankkontonummer når du bruker en DLP-sensitiv informasjonstype i O365?  Hvis dette er det, må du kontrollere at innholdet inneholder den nødvendige informasjonen for hva DLP-policyen ser etter når den evalueres.
  
For en policy  for amerikansk bankkontonummer som er konfigurert med et konfidensnivå på 85 %, evalueres for eksempel følgende og må oppdages for at regelen skal utløse:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8–17 sifre

- **[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8–17 etterfølgende sifre.

- **[Sjekksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nei, det finnes ingen Checksum

- **[Definisjon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** En DLP-policy er 75 % sikker på at den har oppdaget denne typen sensitiv informasjon hvis den er i nærheten av 300 tegn:

  - Det vanlige uttrykket Regex_usa_bank_account_number finner innhold som samsvarer med mønsteret

  - Et nøkkelord fra Keyword_usa_Bank_Account finnes.

    Eksempel: Følgende eksempel vil utløse for **policyen** for amerikansk bankkontonummer: Kontrollere kontonummer 78344011

Hvis du vil ha mer  informasjon om hva som kreves for at et amerikansk bankkontonummer skal oppdages for innholdet ditt, kan du se følgende del i denne artikkelen: Hva de sensitive informasjonstypene ser for amerikanske [bankkontonummer?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Hvis du bruker en annen innebygd sensitiv informasjonstype, kan du se følgende artikkel for informasjon om hva som kreves for andre typer: Hva de [sensitive informasjonstypene ser etter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  