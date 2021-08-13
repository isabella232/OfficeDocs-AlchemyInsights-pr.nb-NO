---
title: Overvåke betinget tilgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975110"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Overvåke betinget tilgang for Exchange

Brukere som er målrettet med betinget tilgang, mottar en e-postmelding hvis de ikke oppfyller organisasjonens tilgangskrav. Vi anbefaler én eller flere av følgende løsninger for å løse problemet:

- Hvis enheten antas å være registrert, ber du brukeren om å gå til firmaportal-appen og kontrollere at den vises i firmaportal. Hvis den ikke gjør det, bør brukeren registrere enheten.
- I Azure-portalen går du til Intune > Enhetssamsvar. Klikk Enhetssamsvar under Skjerm. Vis samsvarsrapporten for enheten for å bekrefte at brukerens enhet er merket som kompatibel.
- I Azure-portalen går du til Intune > Enhetssamsvar. Klikk Policyer under Behandle. Kontroller at en profil er tilordnet brukerens enhet i listen over samsvarspolicyer. Hvis ingen profil er tilordnet, kan ikke Intune bekrefte enhetens samsvarsstatus.
- Rediger brukerens tilordning for betinget tilgang.

1. Gå til Policyer for **betinget tilgang i**  >  **Azure-portalen.**  >  
2. Velg en policy fra listen.
3. Klikk Brukere og grupper.
4. Hvis du vil rette en bestemt policy mot noen, legger du dem til i Inkluder-listen. Hvis du vil sikre at en person utelates fra policyen, legger du vedkommende til i Utelat-listen.

Nyttige koblinger:

[Oversikt over enhetssamsvar](https://docs.microsoft.com/intune/device-compliance-get-started)

[Feilsøking av sertifiseringsinstans](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Feilsøkingspolicy](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Overvåke intune-enhetssamsvar](https://docs.microsoft.com/intune/compliance-policy-monitor)

Obs! Disse trinnene er bare nyttige når du skal feilsøke Azure Active Directory funksjonen Betinget tilgang. Det er også mulig å sette en enhet i karantene som blokkerer e-posttilgang med Exchange policy. Du finner Exchange mer informasjon om enhetsbehandling [her]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
