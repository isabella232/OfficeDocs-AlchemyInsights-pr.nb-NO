---
title: Klargjøring av brukere
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004348"
- "8428"
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971348"
---
# <a name="user-provisioning"></a>Klargjøring av brukere

- Bruk den [behovskrevne klargjøringsfunksjonen](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) til å klargjøre en bruker og få detaljert diagnostikk om trinnene som er utført.
- Hvis du vil feilsøke problemer som oppstår når du klargjør brukere og grupper, kan du se feilsøkingsveiledningen [Ingen brukere klargjøres.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Hvis du ser at brukere ikke klargjøres, kan du se [Klargjøringslogger (forhåndsvisning)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) i Azure Active Directory (AD). Søk etter loggoppføringer som gjelder for en bestemt bruker.
- Start klargjøring på nytt med jevne mellomrom for å fange opp eventuelle brukere som ble gått glipp av en tidligere klargjøringssyklus.
- Brukeren/gruppen har kanskje ikke blitt klargjort fordi tjenesten ikke har hatt mulighet til å evaluere brukeren ennå. Se gjennom veiledningen for hvor lang tid klargjøring tar, samt fremdriftslinjen på klargjøringskonfigurasjonssiden. Hvis stødig tilstand angitt i tilleggsdetaljer-delen er før datoen brukeren ble opprettet/oppdatert/slettet, betyr det at vi ikke har evaluert brukeren ennå. I dette scenarioet er det beste å vente til klargjøringstjenesten er ferdig. Hvis den stabile tilstanden er oppnådd, anbefaler vi å utføre en omstart fra brukergrensesnittet i Azure Portal.
  - Vær oppmerksom på at tjenesten vår bare er klar over endringer i en bruker/gruppe i kildesystemet (Azure Active Directory). Hvis en bruker/gruppe fjernes direkte i programmet (for eksempel ServiceNow), er vi ikke klar over disse endringene og ruller den ikke tilbake basert på tilstanden til brukeren i kildesystemet. I dette scenarioet er det best å rulle tilbake endringen direkte i målprogrammet.
- Tjenesten vår evaluerte brukeren/gruppen og fant ut at den ikke skulle klargjøres:
  - Hvis du har angitt omfanget til tilordnede brukere og grupper, kontrollerer du om brukeren/gruppen er tilordnet til programmet.
  - Hvis brukeren/gruppen er tilordnet til programmet, må du kontrollere at de ikke er tilordnet til standard tilgangsrolle. Denne rollen kan ikke brukes til klargjøring.
  - Hvis du har angitt et attributtbasert filtreringsfilter, må du kontrollere at brukeren oppfyller vilkårene du har angitt.
  - Hvis brukere allerede finnes i målsystemet og statusen til brukeren i kilde- og måls samsvaret, vil vi ikke gjøre noe mer.
- Tjenesten forsøkte å klargjøre brukeren, og den mislyktes. Se gjennom feilsøkings- og anbefalinger-fanen i klargjøringsloggene for disse scenariene:
  - Et obligatorisk attributt for brukeren kan mangle i Azure Active Directory eller samsvarer ikke med formatet som kreves av tredjepartsprogrammet. Land-attributtet for en bruker kan for eksempel settes til USA når det skal være USA.
  - Attributtet er et referanseattributt som ennå ikke finnes i målprogrammet. Et referanseattributt er et attributt som peker til et annet objekt, for eksempel en bruker som er medlem av en gruppe. Brukerens ID vil være i medlemsattributtet for gruppen, men kan bare behandles hvis brukerobjektet den peker til, allerede finnes.
