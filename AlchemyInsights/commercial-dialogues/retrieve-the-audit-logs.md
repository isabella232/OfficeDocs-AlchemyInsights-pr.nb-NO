---
title: Hente overvåkingsloggene
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 88d28898923c1381c001c15445da90901b7e8761
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320452"
---
# <a name="retrieve-the-audit-logs"></a>Hente overvåkingsloggene

Når du åpner overvåkingsloggen for første gang, vil den være tom. Du må gjøre et søk for å se hva som er der. Slik gjør du et generelt søk etter alle aktiviteter:

1. Gjør en av følgende handlinger:
   - I Samsvarssenter for Microsoft 365 på <https://compliance.microsoft.com> går du til **Løsningsovervåking** \> . Du kan også gå direkte til **overvåkingssiden** ved å bruke <https://compliance.microsoft.com/auditlogsearch> .
   - Gå Microsoft 365 Defender til Overvåking i <https://security.microsoft.com> **portalen** på . Du kan også gå direkte til **overvåkingssiden** ved å bruke <https://security.microsoft.com/auditlogsearch> .

2. Konfigurer følgende innstillinger  på **Søk-fanen** på overvåkingssiden:
   - **Dato- og klokkeslettområde:** Velg dato-/klokkeslettområdet i **Start-** og **Slutt-boksene.**
   - **Aktiviteter:** Kontroller **at Vis resultater for alle aktiviteter** er valgt.
   - **Brukere:** Godta den tomme standardverdien for å returnere resultater for alle brukere, eller angi én eller flere brukere.

3. Når du er ferdig, klikker du **Søk**. Aktivitetene vises på den nye **siden for overvåkingssøk.**

4. Velg en aktivitet i resultatene for å åpne undermenyen for detaljer. Du vil se mer informasjon, for eksempel Klient, Bruker som utførte handling og så videre.

Hvis du vil ha mer informasjon, kan [du se Søke i overvåkingsloggen for å undersøke vanlige støtteproblemer.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
