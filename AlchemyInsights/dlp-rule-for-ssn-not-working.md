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
ms.openlocfilehash: cfe884a207490a19325ce059652de158c16dc801
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704094"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-problemer med personnummer

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

**DLP-problemer med SSN-er**

Har du problemer med at **dlp (Data Loss Prevention)** ikke fungerer for innhold som inneholder et **personnummer (SSN)** når du bruker en sensitiv informasjonstype i Office 365? I så fall må du kontrollere at innholdet inneholder den nødvendige informasjonen for hva DLP-retningslinjene ser ut. 
  
For en SSN-policy som er konfigurert med et konfidensnivå på 85 %, evalueres følgende for eksempel for at regelen skal utløses:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 sifre, som kan være i et formatert eller uformatert mønster

- **[Mønster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fire funksjoner ser etter SSNer i fire forskjellige mønstre:

  - Func_ssn finner SSNer med sterk formatering før 2011 som er formatert med bindestreker eller mellomrom (dddd-dddd eller ddd dd dddd)

  - Func_unformatted_ssn finner SSNer med sterk formatering før 2011 som ikke er formatert som ni påfølgende sifre (ddddddddddd)

  - Func_randomized_formatted_ssn finner som-koder etter 2011 som er formatert med bindestreker eller mellomrom (dddd-dddd ddd dd dd ddd)

  - Func_randomized_unformatted_ssn finner som-koder etter 2011 som ikke er formatert som ni påfølgende sifre (dddddddddddd)

- **[Sjekksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nei, det er ingen Checksum

- **[Definisjon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** En DLP-policy er 85% sikker på at den oppdages denne typen sensitiv informasjon hvis, i nærheten av 300 tegn:

  - [Funksjonen Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finner innhold som samsvarer med mønsteret.

  - Finner et nøkkelord fra [Keyword_ssn.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) Eksempler på søkeord inkluderer: *Trygd, Trygd#, Soc Sec , SSN* . Følgende eksempel utløses for eksempel DLP SSN-policyen: **SSN: 489-36-8350**
  
Hvis du vil ha mer informasjon om hva som kreves for at SSN-er skal oppdages for innholdet ditt, kan du se følgende del i denne artikkelen: [Hvilke sensitive informasjonstyper ser etter SSN-er](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Hvis du bruker en annen innebygd sensitiv informasjonstype, kan du se følgende artikkel for informasjon om hva som kreves for andre typer: [Hva sensitive informasjonstyper ser etter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  