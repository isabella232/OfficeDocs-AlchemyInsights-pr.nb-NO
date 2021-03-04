---
title: Overvåke Betinget tilgang med Intune
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
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427924"
---
# <a name="monitor-intune-conditional-access"></a>Overvåke Betinget tilgang med Intune

Brukere som er angitt med betinget tilgang, mottar en e-postmelding hvis de ikke oppfyller organisasjonens krav for tilgang. Hvis du vil løse problemet, anbefaler vi én eller flere av følgende løsninger:

1. Hvis det antas at enheten er registrert, ber du brukeren om å gå til Firmaportal-appen og kontrollere at den vises i firmaportalen. Hvis den ikke gjør det, må brukeren registrere enheten.
1. Gå til Enhetssamsvar for **Intune**  >  **i Azure-portalen.** 
1. Hvis du vil vise rapporten om enhetssamsvar for å kontrollere at brukerens enhet er merket som kompatibel, klikker du Enhetssamsvar **under** **Skjerm.**
1. Gå til Enhetssamsvar for **Intune**  >  **i Azure-portalen.** Klikk **Policyer** under **Behandle.** Kontroller at brukerens enhet er tilordnet en profil i listen over samsvarspolicyer. Hvis ingen profil er tilordnet, kan ikke Intune bekrefte enhetens samsvarsstatus.
1. Rediger brukerens tilordning av betinget tilgang.
1. Gå til **Intune-policyer** for betinget tilgang i Azure-portalen, velg en policy fra listen, og klikk  >    >  Brukere **og grupper.**
1. Hvis du vil rette en bestemt policy mot noen, legger du dem til **i Inkluder-listen.** Hvis du vil sikre at en person er utelatt fra policyen, legger du vedkommende til i **utelatingslisten.**

**Nyttige koblinger:**

- [Oversikt over enhetssamsvar](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Feilsøking av sertifiseringsinstans](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Feilsøking av policy](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Overvåke intune-enhetssamsvar](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Disse trinnene er bare nyttige når du skal feilsøke Azure Active Directory-funksjonen betinget tilgang. Det er også mulig å sette en enhet i karantene for å blokkere tilgangen til e-post med Exchange-policy. Du finner mer informasjon om administrasjon av Exchange-enheter [**her.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
