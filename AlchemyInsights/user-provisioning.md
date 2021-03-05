---
title: Klargjøring av bruker
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
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481885"
---
# <a name="user-provisioning"></a>Klargjøring av bruker

- Bruk [klargjøringsfunksjonen ved behov til](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) å klargjøre en bruker og få detaljert diagnose om trinnene som er utført.
- Hvis du vil feilsøke problemer som oppstår under klargjøring av brukere og grupper, kan du se feilsøkingsveiledningen Ingen brukere [klargjøres.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Hvis du ser at brukere ikke klargjøres, kan du se [Klargjøringslogger (forhåndsvisning)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) i Azure Active Directory (AD). Søk etter loggoppføringer som gjelder for en bestemt bruker.
- Klargjøring startes på nytt regelmessig for å fange opp eventuelle brukere som ble oversett i en tidligere klargjøringssyklus.
- Brukeren/gruppen har kanskje ikke blitt klargjort fordi tjenesten ikke har hatt mulighet til å evaluere brukeren ennå. Se gjennom veiledningen for hvor lang tid klargjøringen tar, i tillegg til fremdriftslinjen på konfigurasjonssiden for klargjøring. Hvis jevn status angitt i delen med tilleggsdetaljer er før datoen da brukeren ble opprettet/oppdatert/slettet, betyr det at vi ikke har evaluert brukeren ennå. I dette scenarioet er det best å vente til klargjøringstjenesten er ferdig. Hvis du oppnår jevn status, anbefaler vi at du utfører en omstart fra brukergrensesnittet i Azure Portal.
  - Vær oppmerksom på at tjenesten bare er oppmerksom på endringer i en bruker/gruppe i kildesystemet (Azure Active Directory). Hvis en bruker/gruppe fjernes direkte i programmet (for eksempel ServiceNow), er vi ikke oppmerksomme på disse endringene og ruller den ikke tilbake basert på statusen til brukeren i kildesystemet. I dette scenariet er det best å rulle tilbake endringen direkte i målprogrammet.
- Tjenesten har evaluert brukeren/gruppen og fastslått at den ikke skal klargjøres:
  - Hvis du har angitt omfanget til tilordnede brukere og grupper, må du kontrollere om brukeren/gruppen er tilordnet til programmet.
  - Hvis brukeren/gruppen er tilordnet til programmet, må du kontrollere at de ikke er tilordnet til standard tilgangsrolle. Denne rollen kan ikke brukes til klargjøring.
  - Hvis du har angitt et attributtbasert filter for å angi poengberegning, må du kontrollere at brukeren oppfyller kriteriene du har angitt.
  - Hvis brukere allerede finnes i målsystemet og statusen til brukeren i kilde- og måls samsvarer, vil vi ikke gjøre noe mer.
- Tjenesten prøvde å klargjøre brukeren, og den mislyktes. Se gjennom fanen feilsøking og anbefalinger i klargjøringsloggene for disse scenariene:
  - Et nødvendig attributt for brukeren kan mangle i Azure Active Directory eller samsvarer ikke med formatet som kreves av tredjepartsprogrammet. Land-attributtet for en bruker kan for eksempel settes til USA når det skal være USA.
  - Attributtet er et referanseattributt som ennå ikke finnes i målprogrammet. Et referanseattributt er et attributt som peker til et annet objekt, for eksempel en bruker som er medlem av en gruppe. Brukerens ID vil være i medlemsattributtet for gruppen, men kan bare behandles hvis brukerobjektet det peker til, allerede finnes.
