---
title: Problem med enkeltbruker
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
- "9004687"
- "8469"
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960160"
---
# <a name="problem-with-single-user"></a>Problem med enkeltbruker

- Brukeren har kanskje ikke blitt klargjort fordi tjenesten ikke har hatt mulighet til å evaluere brukeren ennå. Se gjennom veiledningen for hvor lang tid klargjøring tar, samt fremdriftslinjen på klargjøringskonfigurasjonssiden. Hvis stødig tilstand angitt i tilleggsdetaljer-delen er før datoen brukeren ble opprettet/oppdatert/slettet, betyr det at vi ikke har evaluert brukeren ennå. I dette scenarioet er det beste å vente til klargjøringstjenesten er ferdig.

  - Vær oppmerksom på at tjenesten vår bare er klar over endringer til en bruker i kildesystemet (Sky-HR). Det må være en gyldig endring i kildesystemet for Azure AD for å oppdage endringen og flyte den til Active Directory.
- Klargjøringstjenesten evaluerte brukeren og fant ut at den ikke skulle klargjøres:
  - Hvis du har angitt et attributtbasert filtreringsfilter, må du kontrollere at brukeren oppfyller vilkårene du har angitt.
  - Hvis brukere allerede finnes i målsystemet og statusen til brukeren i kilde- og måls samsvaret, vil vi ikke gjøre noe mer.
- Klargjøringstjenesten forsøkte å klargjøre brukeren, og den mislyktes. Se gjennom feilsøkings- og anbefalinger-fanen i klargjøringsloggene for disse scenariene:
  - Et obligatorisk attributt for brukeren kan mangle i lokal Active Directory eller Azure AD. Genereringsreglene userPrincipalName eller sAMAccountName genererer for eksempel ikke riktig verdi.
  - Det samsvarende attributtet (vanligvis employeeId) løses ikke til en unik bruker i lokal Active Directory eller Azure AD. Det finnes for eksempel to brukere med samme ansatt-ID i AD, og tjenesten returnerer en feilkode som angir dupliserte måloppføringer for samme kildeoppføring.

Hvis du vil se gjennom logger for enkeltbrukere og grupper, kan du se Se gjennom [klargjøringsloggene for](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)et problem med en bestemt bruker.
