---
title: DLP-regel for amerikansk/britisk Passport-nummer fungerer ikke
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
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679233"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemer med DLP-US/Storbritannia Passport-numre

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

**DLP-problemer med amerikanske/britiske Passport-numre**

Har du problemer med tap av datatap **(DLP)** fungerer ikke for innhold som inneholder et **amerikansk/britisk Passport-nummer** når du bruker en DLP sensitiv informasjons type i O365? Hvis det er tilfelle, må du kontrollere at innholdet inneholder den nødvendige informasjonen for hva DLP-policyen ser ut når den evalueres.
  
Hvis du for eksempel har konfigurert en **US/Storbritannia Passport Number-** policy med et konfidenskoeffisienten-nivå på 75%, evalueres følgende og må oppdages for at regelen skal utløse
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Ni sifre

- **[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Ni påfølgende sifre

- **[Kontroll sum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nei, det er ingen kontroll sum

- **[Definisjon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** En DLP-policy er 75% sikker på at den har funnet denne typen sensitiv informasjon hvis, innenfor en nærhet av 300-tegn:

  - Funksjonen Func_usa_uk_passport finner innhold som Sams varer med mønsteret.

  - Et nøkkel ord fra Keyword_passport blir funnet.

    Følgende eksempel vil for eksempel utløse den **amerikanske/britiske Passport Number** -policyen: amerikansk pass nummer 123456789

Hvis du vil ha mer informasjon om hva som kreves for at et amerikansk/britisk Passport-nummer skal oppdages for innholdet, kan du se følgende avsnitt i denne artikkelen: [hva de sensitive informasjons typene ser ut for amerikansk/britisk Passport-nummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Hvis du bruker en annen innebygd sensitiv informasjons type, kan du se følgende artikkel for informasjon om hva som er nødvendig for andre typer: [hva de sensitive informasjons typene ser etter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  