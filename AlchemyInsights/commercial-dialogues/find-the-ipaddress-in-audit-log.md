---
title: Finne IP-adressen i overvåkingsloggen
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
ms.openlocfilehash: c3b1cac5379f4f3da93152fa20086068f7df562cd98b2980ce1b4280e0aa6d5f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57902269"
---
# <a name="find-the-ip-address-in-audit-log"></a>Finne IP-adressen i overvåkingsloggen

IP-adressen som tilsvarer en aktivitet som utføres av en bruker eller administrator, vises i overvåkingsloggene. Klientinformasjonen logges også. Slik identifiserer du IP-adressen:

1. Gjør en av følgende handlinger:
   - I Samsvarssenter for Microsoft 365 på <https://compliance.microsoft.com> går du til **Løsningsovervåking** \> . Du kan også gå direkte til **overvåkingssiden** ved å bruke <https://compliance.microsoft.com/auditlogsearch> .
   - Gå til Microsoft 365 Defender i <https://security.microsoft.com> **portalen** på . Du kan også gå direkte til **overvåkingssiden** ved å bruke <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Hvis du ser et varsel om at du må aktivere overvåking, kan du aktivere den nå. Hvis denne funksjonen ikke er aktivert, kan ikke søkeresultatene hente data fra tidligere datoer.

2. Kontroller at **Søk-fanen**  er valgt på Overvåking-siden, og konfigurer deretter følgende innstillinger:
   - **Dato- og klokkeslettområde:** Velg dato-/klokkeslettområdet i **Start-** og **Slutt-boksene.**
   - **Aktiviteter:** Hvis du er interessert i en bestemt aktivitet, velger du den fra listen. Ellers returneres standardverdien **Vis resultater for alle** aktiviteter. Vær oppmerksom på at enkelte aktiviteter kanskje ikke er tilgjengelige for valg. Disse overvåkingselementene returneres imidlertid hvis **Vis resultater for alle aktiviteter** er valgt.
   - **Brukere:** Godta den tomme standardverdien for å returnere resultater for alle brukere, eller angi én eller flere brukere.

3. Når du er ferdig, klikker du **Søk**. Aktivitetene vises på den nye **siden for overvåkingssøk.**

4. Klikk Filtrer resultater **i** resultatene, og skriv inn **Set-Mailbox** i aktivitetsfilterboksen.

5. Velg en overvåkingspost i resultatene for å åpne **Detaljer-undermenyen.**

Hvis du vil ha mer informasjon, kan du [se Søke i overvåkingsloggen for å undersøke vanlige støtteproblemer.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
