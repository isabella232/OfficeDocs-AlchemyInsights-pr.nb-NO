---
title: DLP-regel for PASSnummer for USA/STORBRITANNIA fungerer ikke
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
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507307"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemer med DLP - AMERIKANSKE / BRITISKE passnummer

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

**DLP-problemer med passnumre i USA/Storbritannia**

Har du problemer med **at Data Loss Prevention (DLP)** ikke fungerer for innhold som inneholder et **amerikansk/britisk passnummer** når du bruker en DLP-sensitiv informasjonstype i O365? I så fall må du kontrollere at innholdet inneholder den nødvendige informasjonen for hva DLP-policyen ser etter når det evalueres.
  
For en policy for **passnummer i USA/Storbritannia** som er konfigurert med et konfidensnivå på 75 %, evalueres følgende og må oppdages for at regelen skal utløses
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Ni sifre

- **[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Ni sifre på rad

- **[Sjekksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nei, det er ingen kontrollsum

- **[Definisjon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** En DLP-policy er 75 % sikker på at den oppdages denne typen sensitiv informasjon hvis, i nærheten av 300 tegn:

  - Funksjonen Func_usa_uk_passport finner innhold som samsvarer med mønsteret.

  - Du finner et nøkkelord fra Keyword_passport.

    Følgende eksempel utløses for eksempel for retningslinjene for passnummer i **USA/Storbritannia:** US Passport-nummer 123456789

Hvis du vil ha mer informasjon om hva som kreves for at et amerikansk/britisk passnummer skal oppdages for innholdet ditt, kan du se følgende del i denne artikkelen: [Hva sensitive informasjonstyper ser etter us/uk passportnummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Hvis du bruker en annen innebygd sensitiv informasjonstype, kan du se følgende artikkel for informasjon om hva som kreves for andre typer: [Hva sensitive informasjonstyper ser etter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  