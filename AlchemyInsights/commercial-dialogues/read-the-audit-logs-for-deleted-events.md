---
title: Les overvåkingsloggene for slettede hendelser
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
ms.openlocfilehash: ec8f845f599e397814bc9077c3fe59edb5324192
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324742"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Les overvåkingsloggene for slettede hendelser

Slik gjør du dette:

1. Gjør en av følgende handlinger:
   - I Samsvarssenter for Microsoft 365 på <https://compliance.microsoft.com> går du til **Løsningsovervåking** \> . Du kan også gå direkte til **overvåkingssiden** ved å bruke <https://compliance.microsoft.com/auditlogsearch> .
   - Gå til Microsoft 365 Defender -portalen <https://security.microsoft.com> på . Du kan også gå direkte til **overvåkingssiden** ved å bruke <https://security.microsoft.com/auditlogsearch> .

    **Obs!** Hvis du ser et varsel om at du må aktivere funksjonen, kan du slå den på nå. Hvis funksjonen ikke er aktivert, kan ikke søkeresultatene hente data fra tidligere datoer.

2. Konfigurer følgende innstillinger  på **Søk-fanen** på overvåkingssiden:
   - **Dato- og klokkeslettområde:** Velg dato-/klokkeslettområdet i **Start-** og **Slutt-boksene.**
   - **Aktiviteter:** **Skriv Exchange aktiviteter i postboksen,** og velg deretter følgende verdier:
     - **Slettede meldinger fra Slettede elementer-mappen**
     - **Flyttet meldinger til Slettede elementer-mappen**

       Når du er ferdig, klikker du utenfor ruten for å minimere **Aktiviteter-ruten.**

   - **Brukere:** Godta den tomme standardverdien for å returnere resultater for alle brukere, eller angi én eller flere brukere.

3. Når du er ferdig, klikker du **Søk**. Aktivitetene vises på den nye **siden for overvåkingssøk.**

4. Velg en aktivitet i resultatene for å åpne undermenyen for detaljer. Tilleggsinformasjon om det slettede elementet, for eksempel emnelinjen og plasseringen av elementet da det ble slettet, vises i **AffectedItems-feltet.**

   **Obs!** Du kan ikke gjenopprette slettede elementer ved hjelp av overvåkingsloggfunksjonen. Hvis du vil gjenopprette slettede elementer, kan du se [Gjenopprette slettede e-postmeldinger i Outlook på nettet](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11).

Hvis du vil ha mer informasjon, kan du [se Søke i overvåkingsloggen for å undersøke vanlige støtteproblemer.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
