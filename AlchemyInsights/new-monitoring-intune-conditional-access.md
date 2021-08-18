---
title: Overvåk Betinget tilgang for Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: 2c3a382671ac95ecbaec1b374bd8c474cf9690a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327566"
---
# <a name="monitor-intune-conditional-access"></a>Overvåk Betinget tilgang for Intune

Brukere som er målrettet med betinget tilgang, mottar en e-postmelding hvis de ikke oppfyller organisasjonens tilgangskrav. Vi anbefaler én eller flere av følgende løsninger for å løse problemet:

1. Hvis enheten antas å være registrert, ber du brukeren om å gå til firmaportal-appen og kontrollere at den vises i firmaportal. Hvis den ikke gjør det, må brukeren registrere enheten.
1. Gå til **Intune** Device compliance i Azure-portalen.  >   
1. Hvis du vil vise samsvarsrapporten for enheten for å bekrefte at brukerens enhet er merket som kompatibel, **klikker** du Enhetssamsvar under **Skjerm**.
1. Gå til **Intune** Device compliance i Azure-portalen.  >   Klikk **Policyer** under **Behandle.** Kontroller at en profil er tilordnet brukerens enhet i listen over samsvarspolicyer. Hvis ingen profil er tilordnet, kan ikke Intune bekrefte enhetens samsvarsstatus.
1. Rediger brukerens tilordning av betinget tilgang.
1. Gå til Policyer for **betinget** tilgang i Azure-portalen, velg en policy fra  >    >  listen, og klikk **Brukere og grupper**.
1. Hvis du vil rette en bestemt policy mot noen, legger du dem til i **Inkluder-listen**. Hvis du vil sikre at en person utelates fra policyen, legger du vedkommende til i **Utelat-listen**.

**Nyttige koblinger:**

- [Oversikt over enhetssamsvar](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Feilsøking av sertifiseringsinstans](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Feilsøkingspolicy](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Overvåke intune-enhetssamsvar](https://docs.microsoft.com/intune/compliance-policy-monitor)

**Obs!** Disse trinnene er bare nyttige når du skal feilsøke Azure Active Directory funksjonen Betinget tilgang. Det er også mulig å sette en enhet i karantene som blokkerer e-posttilgang med Exchange policy. Du finner mer Exchange informasjon om enhetsbehandling [**her**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
