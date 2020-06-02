---
title: DLP-regel for SSN fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507379"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-problemer med personnummer

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

**DLP-problemer med SSN-er**

Har du problemer med **at Data Loss Prevention (DLP)** ikke fungerer for innhold som inneholder et **SSN (Social Security Number)** når du bruker en sensitiv informasjonstype i Microsoft 365? I så fall må du kontrollere at innholdet inneholder den nødvendige informasjonen for hva DLP-retningslinjene ser ut. 
  
For en SSN-policy som er konfigurert med et konfidensnivå på 85 %, evalueres følgende og må oppdages for at regelen skal utløses:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 sifre, som kan være i et formatert eller uformatert mønster

- **[Mønster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fire funksjoner ser etter SSNer i fire forskjellige mønstre:

  - Func_ssn finner SSNer med før 2011 sterk formatering som er formatert med bindestreker eller mellomrom (ddd-dddd ELLER ddd ddd ddddd)

  - Func_unformatted_ssn finner SSNer med før 2011 sterk formatering som er uformatert som ni påfølgende sifre (ddddddddd)

  - Func_randomized_formatted_ssn finner SSN-er etter 2011 som er formatert med bindestreker eller mellomrom (ddd-dddd ELLER ddd ddd ddddd)

  - Func_randomized_unformatted_ssn finner SSNer etter 2011 som ikke er formatert som ni påfølgende sifre (ddddddddd)

- **[Sjekksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nei, det er ingen kontrollsum

- **[Definisjon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** En DLP-policy er 85 % sikker på at den oppdages denne typen sensitiv informasjon hvis, i nærheten av 300 tegn:

  - [Funksjonen Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finner innhold som samsvarer med mønsteret.

  - Du finner et nøkkelord fra [Keyword_ssn.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) Eksempler på nøkkelord inkluderer: *Social Security, Social Security#, Soc Sec , SSN* . Følgende eksempel utløses for eksempel for DLP SSN-policyen: **SSN: 489-36-8350**
  
Hvis du vil ha mer informasjon om hva som kreves for at SSNer skal oppdages for innholdet ditt, kan du se følgende del i denne artikkelen: [Hva sensitive informasjonstyper ser etter SSNer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Hvis du bruker en annen innebygd sensitiv informasjonstype, kan du se følgende artikkel for informasjon om hva som kreves for andre typer: [Hva sensitive informasjonstyper ser etter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  