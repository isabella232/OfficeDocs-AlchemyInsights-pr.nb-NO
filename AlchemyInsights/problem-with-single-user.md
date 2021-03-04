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
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430201"
---
# <a name="problem-with-single-user"></a>Problem med enkeltbruker

- Brukeren har kanskje ikke blitt klargjort fordi tjenesten ikke har hatt mulighet til å evaluere brukeren ennå. Se gjennom veiledningen for hvor lang tid klargjøringen tar, i tillegg til fremdriftslinjen på konfigurasjonssiden for klargjøring. Hvis den stabile tilstanden som er angitt i delen med tilleggsdetaljer er før datoen da brukeren ble opprettet/oppdatert/slettet, betyr det at vi ikke har evaluert brukeren ennå. I dette scenarioet er det best å vente til klargjøringstjenesten er ferdig.

  - Vær oppmerksom på at tjenesten vår bare er oppmerksom på endringer til en bruker i kildesystemet (Cloud HR). Det må være en gyldig endring i kildesystemet for Azure AD for å oppdage endringen og flyte den inn i Active Directory.
- Klargjøringstjenesten evaluert brukeren og bestemte at den ikke skal klargjøres:
  - Hvis du har angitt et attributtbasert filter for å angi poengberegning, må du kontrollere at brukeren oppfyller kriteriene du har angitt.
  - Hvis brukere allerede finnes i målsystemet og statusen til brukeren i kilde- og måls samsvarer, vil vi ikke gjøre noe mer.
- Klargjøringstjenesten prøvde å klargjøre brukeren, og den mislyktes. Se gjennom fanen feilsøking og anbefalinger i klargjøringsloggene for disse scenariene:
  - Et nødvendig attributt for brukeren kan mangle lokalt i Active Directory eller Azure AD. Genereringsreglene userPrincipalName eller sAMAccountName genererer for eksempel ikke den riktige verdien.
  - Attributtet som samsvarer (vanligvis ansattId), løses ikke til en unik bruker i lokal Active Directory eller Azure AD. Det er for eksempel to brukere med samme ansatt-ID i AD, og tjenesten returnerer en feilkode som angir dupliserte måloppføringer for samme kildeoppføring.

Hvis du vil se gjennom logger for enkeltbrukere og grupper, kan du se se gjennom [klargjøringsloggene for et problem med en bestemt bruker.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
