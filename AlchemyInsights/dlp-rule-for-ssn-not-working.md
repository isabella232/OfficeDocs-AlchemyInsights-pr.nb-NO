---
title: DLP-regel for SSN fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: fffd355279b064b31c0a8bf60518b15ee1ed1848
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389442"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-problemer med personnumre

Har du problemer med **Data tap forebygging (DLP)** fungerer ikke for innhold som inneholder et **Personnummer (SSN)** når du bruker en type sensitiv informasjon i Office 365? I så fall må du kontrollere at innholdet inneholder nødvendig informasjon for det DLP-policyen er ute. 
  
For eksempel for en SSN-policy er konfigurert med en konfidenskoeffisienten for 85%, følgende blir evaluert, og må registreres for at regelen skal utløse:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 sifre, noe som kan være i en formatert eller uformatert mønster

- **[Mønster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fire funksjoner se etter SSNs i fire ulike mønstre:

  - Func_ssn søker etter SSNs med pre-2011 Sterk formatering som er formatert med bindestreker eller mellomrom (ddd-dd-dddd eller ddd dd dddd)

  - Func_unformatted_ssn søker etter SSNs med pre-2011 Sterk formatering som er formatert med ni etterfølgende sifre (ddddddddd)

  - Func_randomized_formatted_ssn søker etter post-2011-SSNs som er formatert med bindestreker eller mellomrom (ddd-dd-dddd eller ddd dd dddd)

  - Func_randomized_unformatted_ssn søker etter post-2011-SSNs som er formatert med ni etterfølgende sifre (ddddddddd)

- **[Kontrollsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nei, det finnes ingen kontrollsum

- **[Definisjon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP-policy er 85% sikker på at det har oppdaget at sensitive opplysninger hvis, i en avstand på 300 tegn:

  - [Funksjonen Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) søker etter innhold som samsvarer med mønsteret.

  - Det finnes et nøkkelord fra [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) . Eksempler på nøkkelord inkluderer: *Social Security, Trygd #, Orb sek, Personnummeret* . Hvis du for eksempel følgende eksempel vil utløse for policyen DLP SSN: **SSN: 489-36-8350**
  
Hvis du vil ha mer informasjon om hva som er nødvendig for SSNs blir registrert for innholdet, kan du se delen nedenfor i denne artikkelen: [Hva the Sensitive informasjonstyper se etter SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Å bruke en annen innebygd sensitiv informasjon, se følgende artikkel for å få informasjon på det som er nødvendig for andre typer: [se hva den Sensitive informasjonstyper](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  