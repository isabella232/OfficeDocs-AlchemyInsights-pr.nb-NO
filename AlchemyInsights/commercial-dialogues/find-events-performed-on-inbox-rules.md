---
title: Finne hendelser som er utført på innboksregler
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
ms.openlocfilehash: 626bd7515270f03e1560a3ed637e7bc60b374c5525527205d5f6775e4758f07a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57882644"
---
# <a name="find-events-performed-on-inbox-rules"></a>Finne hendelser som er utført på innboksregler

Når innboksregler opprettes, endres eller slettes, registreres hendelsene i overvåkingsloggen. Slik ser du gjennom dem:

1. Gjør en av følgende handlinger:
   - I Samsvarssenter for Microsoft 365 på <https://compliance.microsoft.com> går du til **Løsningsovervåking** \> . Du kan også gå direkte til **overvåkingssiden** ved å bruke <https://compliance.microsoft.com/auditlogsearch> .
   - Gå til Microsoft 365 Defender i <https://security.microsoft.com> **portalen** på . Du kan også gå direkte til **overvåkingssiden** ved å bruke <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Hvis du ser et varsel om at du må aktivere overvåking, kan du aktivere den nå. Hvis denne funksjonen ikke er aktivert, kan ikke søkeresultatene hente data fra tidligere datoer.

2. Konfigurer følgende innstillinger  på **Søk-fanen** på overvåkingssiden:
   - **Dato- og klokkeslettområde:** Velg dato-/klokkeslettområdet i **Start-** og **Slutt-boksene.**
   - **Aktiviteter:** Velg **Ny innboksRegel Opprett innboksregel fra Outlook Web App**

3. Når du er ferdig, klikker du **Søk**. Aktivitetene vises på den nye **siden for overvåkingssøk.**

4. Velg en aktivitet i resultatene for å åpne undermenyen for detaljer. Under **Parametere-delen** kan du se navnet på regelen, betingelsene som er angitt, og handlingene som regelen skal utføre.

Hvis du vil ha mer informasjon, kan [du se Søke i overvåkingsloggen for å undersøke vanlige støtteproblemer.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
