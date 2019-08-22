---
title: DLP-regel for USA / UK passnummer fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bc91af8be58d49204f84cd7d22f481348af3c013
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529928"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemer med DLP - USA / UK Passport tall

Har du problemer med **Data tap forebygging (DLP)** fungerer ikke for innhold som inneholder en **US / UK passnummer** når du bruker en type for DLP sensitiv informasjon i O365? Hvis dette er tilfelle, kontroller at innholdet inneholder nødvendig informasjon for det DLP-policyen er ute etter når de evalueres.
  
For eksempel for en **US / UK passnummer** policy som er konfigurert med en konfidenskoeffisienten for 75% følgende evalueres og må registreres for at regelen skal utløse
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Ni sifre

- **[Mønster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Ni etterfølgende sifre

- **[Kontrollsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nei, det finnes ingen kontrollsum

- **[Definisjon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP-policy er 75% sikker på at det har oppdaget at sensitive opplysninger hvis, i en avstand på 300 tegn:

  - Til Func_usa_uk_passport å finne innhold som samsvarer med mønsteret.

  - Det finnes et nøkkelord fra Keyword_passport.

    For eksempel følgende eksempel vil utløse den **US / UK passnummer** policy: amerikansk pass tallet 123456789

For mer informasjon om hva som trengs for en US / UK passnummer kan oppdages for innholdet, kan du se delen nedenfor i denne artikkelen: [Hva den Sensitive informasjonstyper utseende for USA / UK passnummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Å bruke en annen innebygd sensitiv informasjon, se følgende artikkel for å få informasjon på det som er nødvendig for andre typer: [se hva den Sensitive informasjonstyper](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  