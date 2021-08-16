---
title: DLP-regel for amerikansk/britisk passnummer fungerer ikke
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004955"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemer med DLP – passnumre i USA/Storbritannia

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

**DLP-problemer med passnumre i USA/Storbritannia**

Har du problemer med hindring av datatap **(DLP)** som ikke fungerer for innhold som inneholder et passnummer i **USA/Storbritannia** når du bruker en DLP-sensitiv informasjonstype i O365? Hvis dette er det, må du kontrollere at innholdet inneholder den nødvendige informasjonen for hva DLP-policyen ser etter når den evalueres.
  
For en **amerikansk/britisk** passnummerpolicy som er konfigurert med et konfidensnivå på 75 %, evalueres følgende og må oppdages for at regelen skal utløse
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Ni sifre

- **[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Ni etterfølgende sifre

- **[Sjekksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nei, det finnes ingen Checksum

- **[Definisjon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** En DLP-policy er 75 % sikker på at den har oppdaget denne typen sensitiv informasjon hvis den er i nærheten av 300 tegn:

  - Funksjonen Func_usa_uk_passport finner innhold som samsvarer med mønsteret.

  - Et nøkkelord fra Keyword_passport er funnet.

    Følgende eksempel utløser for eksempel **amerikansk/britisk** passnummerpolicy: Amerikansk passnummer 123456789

Hvis du vil ha mer informasjon om hva som kreves for at et amerikansk/britisk passnummer skal oppdages for innholdet ditt, kan du se følgende avsnitt i denne artikkelen: Hva sensitiv informasjonstyper ser [etter amerikansk/britisk passnummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Hvis du bruker en annen innebygd sensitiv informasjonstype, kan du se følgende artikkel for informasjon om hva som kreves for andre typer: Hva de [sensitive informasjonstypene ser etter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  