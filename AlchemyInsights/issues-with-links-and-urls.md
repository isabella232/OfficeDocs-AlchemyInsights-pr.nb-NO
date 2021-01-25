---
title: Problemer med koblinger og URL-adresser
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974760"
---
# <a name="issues-with-links-and-urls"></a>Problemer med koblinger og URL-adresser

Omadresser URI/svar-URL-adresser (begge uttrykkene kan byttes) er URL-adressene som brukes av Microsoft Identity Platform til å returnere apper-forespurte tokens. Hvis du vil ha informasjon om disse URL-adressene, kan du se følgende artikler:

- [Godkjennings flyter og program scenarioer](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – informasjon om omdirigerings-URIene i **app-registrerings** siden for hvert scenario.
- [URL-begrensninger og begrensninger for omdirigering av URI/svar](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Jeg vet ikke hvordan jeg registrerer riktig omdirigerings-URI/svar-URL-adresse for appen**

Når du logger deg på med programmet du utvikler, viser påloggings dialog boksen **AADSTS50011: svar-URL-adressen som er angitt i forespørselen, Sams varer ikke med svar-URL-adressene som <your app ID> er konfigurert for programmet**, du må legge til en omdirigerings-URI som koden som ble brukt i token-forespørselen til Microsoft Identity Platform, i program registreringen.

Hvis du vil legge til en URL-adresse for svar, går du til **godkjenning** -fanen på siden for **program registrering** i Azure-portalen og legger til en oppføring i delen **Omadresser URIer** . Omdirigerings-URIene er skrevet inn (nett eller mobil/stasjonær data maskin). Verdien du må angi, avhenger av typen program du bygger, som beskrevet nedenfor:

- For enkelt side programmer og nett apper er URL-adressen for svar en URL-adresse i programmet. Se [program registrering på én side](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) , eller [Registrer en app for Web App ved hjelp av Azure-portalen](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- For skrive bords programmer avhenger verdien du må velge, på:
    - plattformen (MacOS er forskjellig fra Windows eller Linux)
    - måten du henter tokenet på (interaktivt, med enhets kode flyt, med integrert Windows-godkjenning [IWA] eller med bruker navn/passord).
    Hvis du vil ha mer informasjon, se [skrive bords programmer – program registrering – Omadresser URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- For mobile programmer avhenger omdirigerings-URIEN på:
    - plattformen (iOS/Android/UWP)
    - informasjonen som brukes til å bygge opp appen, for eksempel bunt-ID i iOS, og pakke navnet og signatur nummer på Android i registreringen av Azure Portal-appen hjelper deg. Hvis du vil ha mer informasjon, se [Platform Configuration and redirect URIer](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Nett-APIer og noen av de stillende måtene ved å skaffe tokener (IWA og bruker navn/passord) krever ikke en omdirigerings-URI.

**Jeg har distribuert web programmet, og når jeg tester den distribuerte appen, får jeg en melding om manglende samsvar I URL-adresse**

Legg til omdirigerings-URIer for alle plasseringene der du distribuerer nett programmet. Hvis du vil ha mer informasjon, kan du se [registrere et Web App-program ved hjelp av Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Legg til URI for omadressering for en plassering umiddelbart etter at du har distribuert programmet på denne plasseringen.

**Jeg kan ikke registrere nok URL-adresser for svar**

Du er en ISV og har én eller flere omdirigerings-URIer for hver kunde i dine. Du vil overføre fra ADAL/Azure AD v 1.0 til MSAL/Microsoft Identity Platform, og du treffer [maksimalt antall omdirigerings-URIer](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Du kan løse dette ved å [legge til omdirigerings-URIer i tjeneste objekter](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) som Sams varer med hver av kundene dine.
