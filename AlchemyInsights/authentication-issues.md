---
title: Godkjennings problemer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 53bd0d8f8edaead519d0282239d3a6d338b297b9
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974785"
---
# <a name="authentication-issues"></a>Godkjennings problemer

**Leter du etter informasjon om AADSTS-feilkodene som returneres fra Azure Active Directory (STS) for sikkerhets kode (Azure AD)?** Se [Azure ad Authentication and Authorization Error Codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) for å finne AADSTS-feil beskrivelser, løsninger og noen foreslåtte løsninger.

Godkjennings feil kan være et resultat av flere forskjellige problemer, som oftest genererer en 401-eller 403-feil. Følgende problemer kan for eksempel føre til godkjennings feil:

- Feil [innhentings flyt for token](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) for tilgangstoken 
- Dårlig konfigurerte [tillatelses omfang](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Mangel på [samtykke](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Hvis du vil løse vanlige godkjennings feil, kan du prøve Fremgangs måten nedenfor som Sams varer best med feilen du mottar. Mer enn ett trinn kan gjelde for en feil du mottar.

- **401 uautorisert feil melding: er tokenet ditt gyldig?**

Kontroller at appen presenterer et gyldig tilgangstoken til Microsoft Graph som en del av forespørselen. Denne feilen betyr ofte at tilgangstoken kan mangle i forespørsels hodet for HTTP-godkjenning, eller at tokenet er ugyldig eller er utløpt. Vi anbefaler på det sterkeste at du bruker Microsoft Authentication Library (MSAL) for å få tilgang til token-innhenting. I tillegg kan denne feilen oppstå hvis du prøver å bruke et delegert tilgangstoken som er gitt til en personlig Microsoft-konto, for å få tilgang til en API som bare støtter jobb-eller skole kontoer (organisasjons kontoer).

**403 forbudt-feil: har du valgt riktig tillatelses sett?**

Kontroller at du har bedt om det riktige tillatelses settet basert på Microsoft Graph-APIene som programmet ringer til. Anbefalte tillatelser med minimums rettigheter finnes i alle emner i referanse metoden for Microsoft Graph API. I tillegg må disse tillatelsene gis til programmet av en bruker eller administrator. Tildeling av tillatelser skjer vanligvis gjennom en tillatelses side eller bruk av avregistrerings blad for Azure Portal-programmet. Klikk **nødvendige tillatelser** fra **Innstillinger** -blad for programmet, og klikk deretter **gi tillatelser**. Hvis du vil ha mer informasjon, kan du se:

- [Microsoft Graph-tillatelser](https://docs.microsoft.com/graph/permissions-reference) 
- [Lære om Azure AD-tillatelser og samtykke](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 forbudt-feil: ble appen hentet et token for å samsvare med valgte tillatelser?**

Kontroller at typene tillatelser som ble forespurt eller innvilget, Sams varer med typen tilgangs kode som appen henter. Du ber kanskje om å gi app-tillatelser, men bruker delegerte interaktive Code Flow-tokener i stedet for klient legitimasjons flyt tokener, eller ber om og gir delegert tillatelse, men bruker tokener for klient legitimasjons flyt i stedet for delegerte kode flyt tegn.

Hvis du vil ha mer informasjon om hvordan du henter tokener, kan du se:

- [Få tilgang på vegne av brukere og Delegerte tillatelser](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v 2.0-OAuth 2,0 Autorisasjons kode flyt](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Få tilgang uten en User (Daemon-tjeneste) og program tillatelser](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v 2.0 – OAuth 2,0 klient legitimasjons flyt](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 forbudt-feil: tilbakestille passordet**

For øyeblikket er det ingen tillatelse for tjeneste-til-tjeneste-Daemon for program tillatelse som tillater tilbakestilling av bruker passord. Disse APIene støttes bare ved hjelp av den interaktive delegerte koden som flyter med en pålogget administrator. Hvis du vil ha mer informasjon, kan du se [Microsoft Graph-tillatelser](https://docs.microsoft.com/graph/permissions-reference).

**403 forbudt: har brukeren tilgang og er de lisensiert?**

For delegert kode flyter evaluerer Microsoft Graph om forespørselen er tillatt, basert på tillatelsene som ble gitt til appen, og tillatelsene som den påloggede brukeren har. Vanligvis indikerer denne feilen at brukeren ikke er privilegert nok til å utføre forespørselen, **eller** fordi brukeren ikke er lisensiert for dataene du har tilgang til. Bare brukere med de nødvendige tillatelsene eller lisensene kan gjøre forespørselen utført.

**403 forbudt: har du valgt riktig ressurs-API?**

API-tjenester som Microsoft Graph Kontroller at *AUD* -krav (mål gruppe) i mottatt tilgangstoken Sams varer med verdien den forventer for seg selv, og hvis ikke, oppstår det en 403-feil. En vanlig feil som resulterer i denne feilen, prøver å bruke et token som skaffes for Azure AD Graph-APIer, Outlook-APIer eller SharePoint/OneDrive-APIer for å ringe Microsoft Graph (eller omvendt). Kontroller at ressursen (eller omfanget) som programmet ditt henter et token for, Sams varer med APIEN som appen ringer.

**400 Ugyldig forespørsel eller 403 forbudt: bruker brukeren til å overholde organisasjonens policyer for betinget tilgang (CA)?**

Basert på organisasjonens policyer for betinget tilgang (CA), kan en bruker som har tilgang til Microsoft Graph-ressurser via appen, bli Challenged for mer informasjon som ikke finnes i tilgangstoken som programmet opprinnelig anskaffet. I dette tilfellet mottar appen en **400 med en *interaction_required*** -feil under token-innhenting eller en **403 med *Insufficient_claims*** feil når du ringer til Microsoft Graph. I begge tilfeller inneholder feil svaret tilleggs informasjon som kan presenteres for det autoriserte ende punktet for å utfordre brukeren for mer informasjon (for eksempel godkjenning av flere faktorer eller enhets registrering).

Hvis du vil ha mer informasjon om betinget tilgang, kan du se:

- [Behandling av betingede tilgang](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Veiledning for utvikler for Azure Active Directory betinget tilgang](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Slutten av støtte for Azure Active Directory Authentication Library (ADAL) og Azure ad Graph API (AAD-graf)_* _

- Fra og med 30. juni 2020 vil vi ikke lenger legge til nye funksjoner i Azure Active Directory Authentication Library (ADAL) og Azure AD Graph API (AAD-graf). Vi vil fortsette å gi tekniske støtte og sikkerhets oppdateringer, men vil ikke lenger gi funksjons oppdateringer.
- Fra og med 30. juni 2022 vil vi avslutte støtte for ADAL og AAD-graf og vil ikke lenger gi tekniske støtte eller sikkerhets oppdateringer.
    - Apper som bruker ADAL på eksisterende OS-versjoner vil fortsatt fungere etter denne tiden, men får ingen tekniske støtte eller sikkerhets oppdateringer.
    - Apper som bruker AAD Graph etter dette tidspunktet, vil kanskje ikke lenger motta svar fra ende punktet til AAD-grafen.

_ *ADAL-overføring**

Vi anbefaler at du oppdaterer til [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de nyeste funksjonene og sikkerhets oppdateringene. Denne anbefalingen er i omgivelsene til Microsoft som overfører sine programmer til MSAL ved hjelp av tids fristen for slutt på støtte. Formålet med Microsoft-programmenes overføring til MSAL er å sikre at appene drar nytte av MSALs forbedringer i kontinuerlig sikkerhet og funksjoner.

- [Les ADAL vanlige spørsmål](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Lær om hvordan du overfører apper på en per-plattform-basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Hvis du trenger hjelp til å forstå hvilke av appene som bruker ADAL, anbefaler vi at du ser gjennom alle appenes kilde kode, og hvis det er aktuelt, kan du nå ut til alle uavhengige program vare leverandører (ISV) eller program leverandører. Microsoft kunde støtte kan også gi deg en liste over alle ikke-Microsoft-ADAL-apper i leieren din.

**Overføring av AAD-graf**

For programmer som bruker AAD-grafen, følger du veiledningen vår for å [overføre apper i Azure ad Graph til Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Overførings sjekk listen vår gir et komme i gang-punkt](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Registrerings portalen for Azure-apper viser hvilke programmer som bruker AAD-graf. Vi anbefaler at du ser gjennom alle appenes kilde kode, og hvis det er aktuelt, kan du nå ut til alle uavhengige program vare leverandører. Microsoft kunde støtte kan også gi deg informasjon om all bruk av AAD-graf i leieren din.

 










