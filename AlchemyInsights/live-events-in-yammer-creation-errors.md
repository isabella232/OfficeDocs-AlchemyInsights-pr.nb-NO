---
title: Feil ved opprettelse av direktesendte arrangementer i Yammer
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
- "9002495"
- "5112"
ms.openlocfilehash: 383943d670c935403fb7f4466a72474120e27e7a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825524"
---
# <a name="live-events-in-yammer-creation-errors"></a>Feil ved opprettelse av direktesendte arrangementer i Yammer

**Opprettelse av direktesendte arrangementer i Yammer**

Yammer viser til enhver tid alternativet for å opprette et direktesendt arrangement. I noen tilfeller kan det hende at en bruker ikke oppfyller kravene for å kunne opprette et direktesendt arrangement og får en feilmelding når de prøver å opprette det. Nedenfor finner du de vanligste årsakene til dette problemet, og måter å løse det for sluttbrukere.

**Hvem kan opprette direktesendte arrangementer**
- En Office 365 Enterprise E1-, E3-eller E5-lisens eller en Office-365 A3-eller A5-lisens.
- Tillatelse til å opprette direktesendte arrangementer i administrasjonssenteret for Microsoft Teams.
- Tillatelse til å opprette direktesendte arrangementer i Microsoft Stream (for hendelser som produseres ved bruk av en ekstern kringkastingsapp eller enhet).
- Fullstendig gruppemedlemskap i organisasjonen (kan ikke være en gjest eller fra en annen organisasjon).
- Privat møtetidsplan, skjermdeling og deling av IP-video, aktivert i gruppemøtepolicyen.

**Policyer for opprettelse av direktesendte arrangementer**

Yammer følger policyer for direktesendte arrangementer som er angitt i Office 365-tenant for Stream. Alle i organisasjonen kan opprette direktesendte arrangementer som standard. Administratorer kan [gjøre endringer i denne innstillingen, noe som kan hindre brukere i å opprette et direktesendt arrangement](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating). Det er viktig å kontrollere at brukerne har tillatelse til å opprette direktesendte arrangementer hvis de får en policy-feil.
