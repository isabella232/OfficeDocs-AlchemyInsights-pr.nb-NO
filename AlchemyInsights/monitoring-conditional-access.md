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
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708683"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Overvåke betinget tilgang for Exchange

Brukere som er angitt med betinget tilgang, mottar en e-postmelding hvis de ikke oppfyller organisasjonens krav for tilgang. Hvis du vil løse problemet, anbefaler vi én eller flere av følgende løsninger:

- Hvis det antas at enheten er registrert, ber du brukeren om å gå til Firmaportal-appen og kontrollere at den vises i firmaportalen. Hvis den ikke gjør det, bør brukeren registrere enheten.
- Gå til Intune > enhetssamsvar i Azure-portalen. Klikk på Enhetssamsvar under Overvåke. Vis rapporten for enhetssamsvar for å kontrollere at brukerens enhet er merket som kompatibel.
- Gå til Intune > enhetssamsvar i Azure-portalen. Klikk Policyer under Behandle. Kontroller at brukerens enhet er tilordnet en profil i listen over samsvarspolicyer. Hvis ingen profil er tilordnet, kan ikke Intune bekrefte enhetens samsvarsstatus.
- Rediger brukerens tilordning av betinget tilgang.

1. Gå til Policyer for betinget tilgang i **Intune**  >  **i Azure-portalen.**  >  
2. Velg en policy fra listen.
3. Klikk Brukere og grupper.
4. Hvis du vil rette en bestemt policy mot noen, legger du dem til i Inkluder-listen. Hvis du vil sikre at en person er utelatt fra policyen, legger du vedkommende til i utelatingslisten.

Nyttige koblinger:

[Oversikt over enhetssamsvar](https://docs.microsoft.com/intune/device-compliance-get-started)

[Feilsøking av sertifiseringsinstans](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Feilsøking av policy](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Overvåke intune-enhetssamsvar](https://docs.microsoft.com/intune/compliance-policy-monitor)

Obs! Disse trinnene er bare nyttige når du skal feilsøke Azure Active Directory-funksjonen for betinget tilgang. Det er også mulig å sette en enhet i karantene for å blokkere tilgang for e-post med Exchange-policy. Du finner mer informasjon om administrasjon av Exchange-enheter [her]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
