---
title: Mottok brukerne skadelig e-post
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 608e2226c055f58ecf4f62e3c913106a6d319190ed6b317508e41514c12ba5d0
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57893412"
---
# <a name="did-your-users-receive-malicious-email"></a>Mottok brukerne skadelig e-post?

Nå kan du rapportere skadelig e-post til Microsoft ved hjelp av [innsendinger i Microsoft 365 Defender portalen.](https://sip.security.microsoft.com/reportsubmission?viewid=admin)

Meldinger som sendes inn i [administratorinnsendinger, skannes,](https://security.microsoft.com/reportsubmission?viewid=admin) og følgende resultater vises i undermenyen for detaljer:

- Hvis det oppstod en feil i avsenderens e-postgodkjenning på leveringstidspunktet.
- Informasjon om eventuelle policy-treff som kan ha påvirket eller overstyrt avgjørelsen til en melding.
- Gjeldende detonasjonsresultater viser om nettadressene eller filene i meldingen var skadelige eller ikke.
- Tilbakemelding fra gradering

Hvis det ble funnet en overstyring, skal den nye skanningen fullføres på noen minutter. Hvis det ikke var et problem med e-postgodkjenning eller hvis leveringen ikke ble påvirket av en overstyring, kan tilbakemeldingen fra gradering ta opptil en dag.

Hvis du er uenig i den endelige avgjørelsen om en melding, nettadresse eller fil (blokkert i stedet for ikke blokkert), send meldingen på nytt etter en dag for ny skanning. Det er store sjanser for at avgjørelsen endres når meldingen sendes på nytt.

I mellomtiden kan du fjerne skadelig e-post fra brukernes innbokser ved å følge instruksjonene i [denne artikkelen](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Kunder med Microsoft Defender for Office 365 kan:
  - Bruke [Trusselutforsker til å finne og slette mistenkelig e-post](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [Bruke Safe koblinger til å blokkere tilgang](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) til en ondsinnet nettadresse
  - Spore brukere som klikket på og fikk tilgang til ondsinnede nettadresser: [Vise nettadressen for phishing, og klikk på kjennelsesdata](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)  &  [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Starte [en automatisert undersøkelse manuelt](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Du kan også beskytte deg mot skadelige filer og nettadresser ved å følge instruksjonene i [Beskyttelse mot skadelige nettadresser og filer](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).
