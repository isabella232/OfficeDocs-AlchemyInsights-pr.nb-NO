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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313508"
---
# <a name="find-events-performed-on-inbox-rules"></a>Finne hendelser som er utført på innboksregler

Når innboksregler opprettes, endres eller slettes, registreres hendelsene i overvåkingsloggen. Slik ser du gjennom dem:

1. Gjør en av følgende handlinger:
   - I Samsvarssenter for Microsoft 365 på <https://compliance.microsoft.com> går du til **Løsningsovervåking** \> . Du kan også gå direkte til **overvåkingssiden** ved å bruke <https://compliance.microsoft.com/auditlogsearch> .
   - Gå til Microsoft 365 Defender -portalen <https://security.microsoft.com> på . Du kan også gå direkte til **overvåkingssiden** ved å bruke <https://security.microsoft.com/auditlogsearch> .

    **Obs!** Hvis du ser et varsel om at du må aktivere overvåking, kan du aktivere det nå. Hvis denne funksjonen ikke er aktivert, kan ikke søkeresultatene hente data fra tidligere datoer.
1. Velg Aktiviteter-feltet, finn Exchange postboksaktiviteter, og velg deretter New-InboxRule Opprett innboksregel fra Outlook Web App. Når du er ferdig, klikker du utenfor ruten for å minimere Aktiviteter-ruten.
1. Angi datoområdet, og velg brukernavnet for brukeren du vil undersøke, i Brukere-feltet. Du kan velge mer enn én bruker om gangen.
1. Velg Søk. Aktivitetene vises under Resultater.
1. Hvis du vil vise detaljer, velger du en aktivitet og velger deretter Mer informasjon. Under Parametere-delen kan du se navnet på regelen, betingelsene som er angitt, og handlingene som regelen skal utføre.

2. Konfigurer følgende innstillinger  på **Søk-fanen** på overvåkingssiden:
   - **Dato- og klokkeslettområde:** Velg dato-/klokkeslettområdet i **Start-** og **Slutt-boksene.**
   - **Aktiviteter:** **Velg Ny innboksRegel Opprett innboksregel fra Outlook Web App**

3. Når du er ferdig, klikker du **Søk**. Aktivitetene vises på den nye **siden for overvåkingssøk.**

4. Velg en aktivitet i resultatene for å åpne undermenyen for detaljer. Under **Parametere-delen** kan du se navnet på regelen, betingelsene som er angitt, og handlingene som regelen skal utføre.

Hvis du vil ha mer informasjon, kan [du se Søke i overvåkingsloggen for å undersøke vanlige støtteproblemer.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
