---
title: Problemer med koblinger og nettadresser
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: d85069970fe6bc6cc7a8488c49c0e6236426d45b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321916"
---
# <a name="issues-with-links-and-urls"></a>Problemer med koblinger og nettadresser

Omdirigerings-URI-er / nettadresser for svar (begge uttrykk kan brukes om hverandre) er nettadressene som brukes av Microsofts identitetsplattform for å returnere appforespurte tokener. Hvis du vil ha informasjon om disse nettadressene, kan du se følgende artikler:

- [Godkjenningsflyter og programscenarioer](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – Informasjon om omdirigerings-URI-ene på **appregistrerings**-siden for hvert scenario.
- [Restriksjoner og begrensninger for omdirigerings-URI / nettadresse for svar](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Jeg vet ikke hvordan jeg registrerer riktig omdirigerings-URI / nettadresse for svar for appen**

Når du logger på med programmet du utvikler, og dialogboksen for pålogging viser **AADSTS50011: Nettadressen for svar som er angitt i forespørselen, samsvarer ikke med nettadressene for svar som er konfigurert for programmet<your app ID>**. Du må legge til programregistreringen, omdirigerings-URI-en som koden brukte i tokenforespørselen, i Microsofts identitetsplattform.

Hvis du vil legge til en nettadresse for svar, går du til **Godkjenning**-fanen på **programregistrerings**-siden i Azure-portalen, og legger til en oppføring i inndelingen **Omdirigerings-URI-er**. Verdien du må skrive inn, avhenger av typen program du bygger, som beskrevet nedenfor:

- Når det gjelder enkeltsideprogrammer og -nettapper, er nettadressen for svar en nettadresse i programmet. Se [Registrering av enkeltsideprogrammer](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) eller [Registrer en nettapp ved hjelp av Azure-portalen](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Når det gjelder skrivebordsapper, avhenger verdien du må velge, av:
    - plattformen (MacOS er forskjellig fra Windows eller Linux)
    - måten du henter tokenet på (interaktivt, med enhetskodeflyt, med integrert Windows-godkjenning [IWA] eller med brukernavn/passord).
    Hvis du vil ha mer informasjon, kan du se [Skrivebordsapper – Appregistrering – Omdirigerings-URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Når det gjelder mobilprogrammer, avhenger omdirigerings-URI-en av:
    - plattformen (iOS/Android/UWP)
    - informasjonen som brukes til å bygge appen, for eksempel bunt-ID-en i iOS, og pakkenavnet og signaturhashen på Android. Azure-portalappregistreringen vil hjelpe deg. Hvis du vil ha mer informasjon, kan du se [Plattformkonfigurasjon og omdirigerings-URI-er](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

**Obs!** Web-API-er og noen av de stille måtene å anskaffe tokener på (IWA og brukernavn/passord) krever ikke en omdirigerings-URI.

**Jeg har distribuert nettprogrammet, og når jeg tester den distribuerte appen, får jeg en samsvarsfeilmelding for nettadresse for svar**

Legg til omdirigerings-URI-er for alle plasseringer der du distribuerer nettprogrammet. Hvis du vil ha mer informasjon, kan du se [Registrer en nettapp ved hjelp av Azure-portalen](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

**Obs!** Legg til omdirigerings-URI for en plassering umiddelbart etter at du har distribuert programmet på denne plasseringen.

**Jeg kan ikke registrere nok nettadresser for svar**

Du er en uavhengig programvareleverandør og har én eller flere omdirigerings-URI-er for hver kunde du har. Du vil overføre fra ADAL/Azure AD v1.0 til MSAL / Microsofts identitetsplattform, og du har nådd [maksimalt antall omdirigerings-URI-er](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Du kan løse dette ved å [legge til omdirigerings-URI-er i tjenestekontohavere](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) som samsvarer med hver av kundene.
