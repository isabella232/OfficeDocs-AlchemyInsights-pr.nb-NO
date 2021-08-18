---
title: Undersøke alle brukernes aktiviteter
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 016f4b1caa05cb26d1e6795551b64737d4cb64a5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332352"
---
# <a name="investigate-all-the-users-activities"></a>Undersøke alle brukernes aktiviteter

Slik gjør du dette:

1. Gjør en av følgende handlinger:
   - I Samsvarssenter for Microsoft 365 på <https://compliance.microsoft.com> går du til **Løsningsovervåking** \> . Du kan også gå direkte til **overvåkingssiden** ved å bruke <https://compliance.microsoft.com/auditlogsearch> .
   - Gå Microsoft 365 Defender til Overvåking i <https://security.microsoft.com> **portalen** på . Du kan også gå direkte til **overvåkingssiden** ved å bruke <https://security.microsoft.com/auditlogsearch> .

    **Obs!** Hvis du ser et varsel om at du må aktivere funksjonen, kan du slå den på nå. Hvis funksjonen ikke er aktivert, kan ikke søkeresultatene hente data fra tidligere datoer.

2. Konfigurer følgende innstillinger  på **Søk-fanen** på overvåkingssiden:
   - **Dato- og klokkeslettområde:** Velg dato-/klokkeslettområdet i **Start-** og **Slutt-boksene.**
   - **Aktiviteter:** Hvis du er interessert i en bestemt aktivitet, velger du den fra listen. Ellers returnerer standardverdien **Vis resultater for alle aktiviteter** alle aktiviteter.
   - **Brukere:** Godta den tomme standardverdien for å returnere resultater for alle brukere, eller angi én eller flere brukere.

3. Når du er ferdig, klikker du **Søk**. Aktivitetene vises på den nye **siden for overvåkingssøk.** Du ser **IP-adressen** **,** bruker- og **aktivitetsnavnet.**

4. Hvis du vil laste ned resultatene, **velger du** \> **Eksporter Last ned alle resultater**.

5. Velg en aktivitet i resultatene for å åpne undermenyen for detaljer.

Hvis du vil ha mer informasjon, kan [du se Søke i overvåkingsloggen for å undersøke vanlige støtteproblemer.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
