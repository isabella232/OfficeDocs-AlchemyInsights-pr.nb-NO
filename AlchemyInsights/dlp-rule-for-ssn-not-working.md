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
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004991"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-problemer med personnumre

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

**DLP-problemer med SSN-er**

Har du problemer med datatapsforhindring **(DLP)** fungerer ikke for innhold som inneholder et personnummer **(SSN)** når du bruker en sensitiv informasjonstype i Microsoft 365? Hvis dette er det, må du kontrollere at innholdet inneholder den nødvendige informasjonen for hva DLP-policyen ser ut. 
  
For en SSN-policy som er konfigurert med et konfidensnivå på 85 %, evalueres for eksempel følgende og må oppdages for at regelen skal utløse:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 sifre, som kan være i et formatert eller uformatert mønster

- **[Mønster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fire funksjoner ser etter SSN-er i fire forskjellige mønstre:

  - Func_ssn finner SSN-er med sterk formatering før 2011 som er formatert med bindestreker eller mellomrom (ddd-dddd ELLER ddd ddd dddd)

  - Func_unformatted_ssn finner SSN-er med sterk formatering før 2011 som ikke er formatert som ni etterfølgende sifre (ddddddddd)

  - Func_randomized_formatted_ssn finner SSN-er etter 2011 som er formatert med bindestreker eller mellomrom (ddd-dddd ELLER ddd dddd)

  - Func_randomized_unformatted_ssn finner SSN-er etter 2011 som ikke er formatert som ni etterfølgende sifre (ddddddddd)

- **[Sjekksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nei, det finnes ingen Checksum

- **[Definisjon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** En DLP-policy er 85 % sikker på at den har oppdaget denne typen sensitiv informasjon hvis den er i nærheten av 300 tegn:

  - Funksjonen [Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finner innhold som samsvarer med mønsteret.

  - Et nøkkelord [fra Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) finnes. Eksempler på nøkkelord omfatter:  *Personnummer, Personnummer#, Soc Sec , SSN*  . Følgende eksempel vil for eksempel utløse for DLP SSN-policyen: **SSN: 489-36-8350**
  
Hvis du vil ha mer informasjon om hva som kreves for at SSN-er skal oppdages for innholdet, kan du se følgende del i denne artikkelen: Hva de sensitive informasjonstypene ser [etter SSN-er?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Hvis du bruker en annen innebygd sensitiv informasjonstype, kan du se følgende artikkel for informasjon om hva som kreves for andre typer: Hva de [sensitive informasjonstypene ser etter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  