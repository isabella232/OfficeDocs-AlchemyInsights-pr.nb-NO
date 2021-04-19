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
ms.openlocfilehash: 425f9ba488fd69b8c5ea29636bccccd995bf48fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815255"
---
# <a name="did-your-users-receive-malicious-email"></a>Mottok brukerne skadelig e-post?

- Nå kan du rapportere skadelig e-post til Microsoft ved hjelp av [Administrasjonsinnsendinger i Sikkerhets- og samsvarssenteret](https://sip.protection.office.com/reportsubmission).

Meldinger som sendes i [administrasjonsinnsendinger](https://sip.protection.office.com/reportsubmission) blir skannet, og følgende resultater vises i **detalj** -undermenyen:

- Hvis det oppstod en feil i avsenderens e-postgodkjenning på leveringstidspunktet.
- Informasjon om eventuelle policy-treff som kan ha påvirket eller overstyrt avgjørelsen til en melding.
- Gjeldende detonasjonsresultater viser om nettadressene eller filene i meldingen var skadelige eller ikke.
- Tilbakemelding fra gradering

Hvis det ble funnet en overstyring, skal den nye skanningen fullføres på noen minutter. Hvis det ikke var et problem med e-postgodkjenning eller hvis leveringen ikke ble påvirket av en overstyring, kan tilbakemeldingen fra gradering ta opptil en dag.

Hvis du er uenig i den endelige avgjørelsen om en melding, nettadresse eller fil (blokkert i stedet for ikke blokkert), send meldingen på nytt etter en dag for ny skanning. Det er store sjanser for at avgjørelsen endres når meldingen sendes på nytt.

I mellomtiden kan du fjerne skadelig e-post fra brukernes innbokser ved å følge instruksjonene i [denne artikkelen](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Kunder med Microsoft Defender for Office 365 kan:
    - bruke [Trusselutforsker til å finne og slette mistenkelig e-post](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [bruke klarerte lenker til å blokkere tilgang ](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) til en skadelig nettadresse
    - spore brukere som klikket og fikk tilgang til skadelige nettadresser: [Vise nettadresse for phishing og klikke avgjørelsesdata](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - manuelt [starte en automatisert undersøkelse](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Du kan også beskytte deg mot skadelige filer og nettadresser ved å følge instruksjonene i [Beskyttelse mot skadelige nettadresser og filer](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).