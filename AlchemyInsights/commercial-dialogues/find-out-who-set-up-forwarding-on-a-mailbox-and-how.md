---
title: Finn ut hvem som konfigurerte videresending på en postboks, og hvordan
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
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317817"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Finn ut hvem som konfigurerte videresending på en postboks, og hvordan

Hvis ekstern videresending ble angitt på en postboks, overvåkes aktiviteten som en del av **cmdleten Set-Mailbox.** Slik finner du aktiviteten i overvåkingsloggen:

1. Gjør en av følgende handlinger:
   - I Samsvarssenter for Microsoft 365 på <https://compliance.microsoft.com> går du til **Løsningsovervåking** \> . Du kan også gå direkte til **overvåkingssiden** ved å bruke <https://compliance.microsoft.com/auditlogsearch> .
   - Gå Microsoft 365 Defender til Overvåking i <https://security.microsoft.com> **portalen** på . Du kan også gå direkte til **overvåkingssiden** ved å bruke <https://security.microsoft.com/auditlogsearch> .

   **Obs!** Hvis du ser et varsel om at du må aktivere overvåking, kan du aktivere det nå. Hvis denne funksjonen ikke er aktivert, kan ikke søkeresultatene hente data fra tidligere datoer.

2. Kontroller at **Søk-fanen**  er valgt på Overvåking-siden, og konfigurer deretter følgende innstillinger:
   - Velg dato-/klokkeslettområdet i **Start-** og **Slutt-boksene.**
   - Kontroller at **Aktiviteter-boksen** inneholder **Vis resultater for alle aktiviteter**.

3. Når du er ferdig, klikker du **Søk**. Aktivitetene vises på den nye **siden for overvåkingssøk.**

4. Klikk Aktivitet-kolonnen  i resultatene for å sortere resultatene, og se etter **Oppføringer i Set-Mailbox.**

5. Velg en aktivitet i resultatene for å åpne undermenyen for detaljer. Du må se på detaljene for hver overvåkingspost for å finne ut om aktiviteten er relatert til videresending av e-post:
   - **ObjectId:** Aliasverdien for postboksen som ble endret.
   - **Parametere:** _ForwardingSmtpAddress_ angir e-postadressen for målet.
   - **UserId:** Brukeren som konfigurerte videresending av e-post på postboksen i **ObjectId-feltet.**

Hvis du vil ha mer informasjon, kan du se [Fastslå hvem som konfigurerte videresending av e-post for en postboks](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
