---
title: DLP-regel for SSN fungerer ikke
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679378"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-problemer med sosiale sikkerhets numre

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

**DLP-problemer med SSNs**

Har du problemer med **tap av datatap (DLP)** fungerer ikke for innhold som inneholder et **person nummer (SSN)** når du bruker en sensitiv informasjons type i Microsoft 365? Hvis det er tilfelle, må du sørge for at innholdet inneholder den nødvendige informasjonen for hva DLP-policyen ser ut. 
  
Hvis du for eksempel har en person som er konfigurert med et visshets nivå på 85%, evalueres følgende og må oppdages for at regelen skal utløse:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 sifre, som kan være i et formatert eller uformatert mønster

- **[Mønster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fire funksjoner ser etter SSNs i fire forskjellige mønstre:

  - Func_ssn finner SSNs med forhånds 2011, sterk formatering som er formatert med binde streker eller mellomrom (DDD-DD-dddd eller DDD DD dddd)

  - Func_unformatted_ssn finner SSNs med forhånds 2011, sterk formatering som ikke er formatert som ni påfølgende sifre (ddddddddd)

  - Func_randomized_formatted_ssn finner SSNs-2011 som er formatert med binde streker eller mellomrom (DDD-DD-dddd eller DDD DD dddd)

  - Func_randomized_unformatted_ssn finner SSNs-2011 som ikke er formatert som ni påfølgende sifre (ddddddddd)

- **[Kontroll sum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nei, det er ingen kontroll sum

- **[Definisjon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** En DLP-policy er 85% sikker på at den har funnet denne typen sensitiv informasjon hvis, innenfor en nærhet av 300-tegn:

  - [Funksjonen Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finner innhold som Sams varer med mønsteret.

  - Et nøkkel ord fra [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) blir funnet. Eksempler på nøkkel ord omfatter:  *sosial sikkerhet, trygd #, SoC SEC, person nummer*  . Følgende eksempel vil for eksempel utløses for DLP SSN-policyen: **SSN: 489-36-8350**
  
Hvis du vil ha mer informasjon om hva som kreves for at SSNs skal oppdages for innholdet, kan du se følgende avsnitt i denne artikkelen: [hva de sensitive informasjons typene ser ut for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Hvis du bruker en annen innebygd sensitiv informasjons type, kan du se følgende artikkel for informasjon om hva som er nødvendig for andre typer: [hva de sensitive informasjons typene ser etter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  