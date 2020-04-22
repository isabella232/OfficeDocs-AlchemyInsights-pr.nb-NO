---
title: DLP-regel for us/UK Passport-nummer fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 9d9615eccd1e245bf4ca32742bfc64321dd7a8cf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714995"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemer med DLP - US / UK passnumre

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

**DLP-problemer med amerikanske/britiske passnumre**

Har du problemer med at **DLP ikke** fungerer for innhold som inneholder et **amerikansk/britisk passnummer** når du bruker en DLP-sensitiv informasjonstype i O365? I så fall må du kontrollere at innholdet inneholder den nødvendige informasjonen for hva DLP-policyen leter etter når det evalueres.
  
For eksempel, for en **amerikansk / britisk passnummerpolicy** konfigurert med et konfidensnivå på 75%, evalueres følgende for at regelen skal utløses
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Ni sifre

- **[Mønster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Ni tall på rad

- **[Sjekksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nei, det er ingen Checksum

- **[Definisjon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** En DLP-policy er 75% sikker på at den oppdages denne typen sensitiv informasjon hvis, i nærheten av 300 tegn:

  - Funksjonen Func_usa_uk_passport finner innhold som samsvarer med mønsteret.

  - Finner et nøkkelord fra Keyword_passport.

    Følgende eksempel utløses for eksempel policyen for passnummer i **USA/Storbritannia:** US Passport-nummer 123456789

Hvis du vil ha mer informasjon om hva som kreves for at et amerikansk/britisk passnummer skal oppdages for innholdet ditt, kan du se følgende avsnitt i denne artikkelen: [Hva sensitive informasjonstyper ser etter us/uk passport nummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Hvis du bruker en annen innebygd sensitiv informasjonstype, kan du se følgende artikkel for informasjon om hva som kreves for andre typer: [Hva sensitive informasjonstyper ser etter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  