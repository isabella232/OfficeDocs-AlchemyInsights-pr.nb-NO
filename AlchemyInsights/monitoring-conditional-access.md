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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366437"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Overvåke betinget tilgang for Exchange

Brukere som er rettet mot betinget tilgang, mottar en e-postvarsling hvis de ikke oppfyller organisasjonens tilgangs krav. Vi anbefaler en eller flere av følgende løsninger for å løse:

- Hvis enheten er Presumed for å bli registrert, ber du brukeren om å gå til Firmaportal-appen og kontrollere at den vises i firma portalen. Hvis den ikke gjør det, skal brukeren registrere enheten.
- I Azure-portalen går du til Intune > enhets samsvar. Under skjerm klikk enhets samsvar. Vis samsvars rapporten for enheten for å bekrefte at brukerens enhet er merket som kompatibel.
- I Azure-portalen går du til Intune > enhets samsvar. Klikk policyer under behandle. Kontroller at en profil er tilordnet til brukerens enhet i listen over samsvars policyer. Hvis ingen profil er tilordnet, vil ikke Intune kunne bekrefte enhetens samsvars status.
- Rediger brukerens tilordningen for betinget tilgang.

1. Gå til **Intune**-policyer for  >  **betinget tilgang**i Azure-portalen  >  **Policies**.
2. Velg en policy fra listen.
3. Klikk brukere og grupper.
4. Hvis du vil angi en bestemt policy for noen, kan du legge dem til i inkluderings listen. Hvis du vil sikre at en person utelates fra policyen, legger du dem til i ekskluderings listen.

Nyttige koblinger:

[Oversikt over enhets samsvar](https://docs.microsoft.com/intune/device-compliance-get-started)

[Feilsøke sertifiserings instans](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Feil søkings policy](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[Overvåke enhets samsvar for Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Obs! disse trinnene er bare nyttige ved feil søking av Azure Active Directory-funksjonen betinget tilgang. Det er også mulig å karantene en enhet som blokkerer e-posttilgang med Exchange-policy. Du finner mer informasjon om administrasjon av Exchange-enheter [her](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).
