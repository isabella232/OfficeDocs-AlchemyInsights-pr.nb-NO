---
title: Godkjenningsproblemer
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
ms.openlocfilehash: c7e6d96940f8d7052ee4b49b22c0d1d7d5bd5f9277f4a7eff709def1da2e13af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019517"
---
# <a name="authentication-issues"></a>Godkjenningsproblemer

**Ser du etter informasjon om AADSTS-feilkoder som returneres fra sikkerhetstokentjenesten for Azure Active Directory (Azure AD) ?** Se[Azure AD Authentication og autorisasjonsfeilkoder](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) for å finne AADSTS-feilbeskrivelser, løsninger og noen foreslåtte midlertidige løsninger.

Autorisasjonsfeil kan være et resultat av flere ulike problemer. De fleste av disse genererer en 401- eller 403-feil. Følgende problemer kan for eksempel alle føre til autorisasjonsfeil:

- Feil [innhentingsflyter for tilgangstoken](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Dårlig konfigurerte [tillatelsesområder](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Mangel på [samtykke](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

For å løse vanlige autorisasjonsfeil kan du prøve trinnene nedenfor som best samsvarer med feilen. Mer enn ett trinn kan gjelde for en feil som du får.

**Feil 401 Uautorisert: Er tokenet gyldig?**

Sørg for at appen presenterer et gyldig tilgangstoken til Microsoft Graph som en del av forespørselen. Denne feilen betyr ofte at tilgangstokenet mangler i forespørselshodet for HTTP-godkjenning, eller at tokenet er ugyldig eller utløpt. Vi anbefaler på det sterkeste at du bruker Microsofts godkjenningsbibliotek (MSAL) for henting av tilgangstoken. I tillegg kan denne feilen oppstå hvis du prøver å bruke et delegert tilgangstoken som er gitt til en personlig Microsoft-konto, til å få tilgang til en API som bare støtter jobb- eller skolekontoer (organisasjonskontoer).

**Feil 403 Ingen tilgang: Har du valgt riktig sett med tillatelser?**

Sørg for at du har bedt om riktig sett med tillatelser basert på Microsoft Graph-API-ene appen kaller opp. Anbefalte minst privilegerte tillatelser er angitt i alle referansemetodeemner for Microsoft Graph-API-en. I tillegg må disse tillatelsene gis til programmet av en bruker eller administrator. Tillatelser blir vanligvis gitt gjennom en samtykkeside eller Azure Portal-programregistreringsbladet. Gå til **Innstillinger**-bladet til programmet, klikk på **Nødvendige tillatelser**, og klikk deretter på **Gi tillatelser**. Hvis du vil ha mer informasjon, kan du se:

- [Microsoft Graph-tillatelser](https://docs.microsoft.com/graph/permissions-reference) 
- [Forstå tillatelse og samtykke for Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**Feil 403 Ingen tilgang: Hentet appen et token for å samsvare med valgte tillatelser?**

Sørg for at typene tillatelse som er forespurt eller gitt, samsvarer med typen tilgangstoken som appen krever. Du ber kanskje om og gi apptillatelser, men bruker delegerte interaktive kodeflyttokener i stedet for klientlegitimasjonsflyttokener, eller du ber om eller gir delegerte tillatelser, men bruker klientlegitimasjonsflyttokener i stedet for delegerte kodeflyttokener.

Hvis du vil ha mer informasjon knyttet til å hente tokener, kan du se:

- [Få tilgang på vegne av brukere og delegerte tillatelser](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 – OAuth 2.0-autorisasjonskodeflyt](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Få tilgang uten en bruker (daemon-tjeneste) og programtillatelser](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 – OAuth 2.0-klientlegitimasjonsflyt](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**Feil 403 Ingen tilgang: Tilbakestilling av passord**

Det er for øyeblikket ingen daemon-tjeneste-til-tjeneste-tillatelser som tillater tilbakestilling av brukerpassord. Disse API-ene støttes bare ved bruk av de interaktive delegerte kodeflytene med en pålogget administrator. Hvis du vil ha mer informasjon, kan du se[Microsoft Graph-tillatelser](https://docs.microsoft.com/graph/permissions-reference).

**403 Ingen tilgang: Har brukeren tilgang og lisens?**

For delegerte kodeflyter evaluerer Microsoft Graph om forespørselen er tillatt basert på tillatelsene som er gitt til appen, og tillatelsene som den påloggede brukeren har. Generelt sett indikerer denne feilen at brukeren ikke har nok rettigheter til å utføre forespørselen, **eller** brukeren er ikke lisensiert for tilgang til dataene. Bare brukere med nødvendige tillatelser eller lisenser kan utføre forespørselen.

**403 Ingen tilgang: Valgte du riktig ressurs-API?**

API-tjenester som Microsoft Graph kontrollerer at *aud*-kravet (målgruppen) i det mottatte tilgangstokenet samsvarer med verdien den forventer for seg selv. Hvis ikke oppstår feilen 403 Ingen tilgang. En vanlig feil som fører til i denne feilen, er å prøve å bruke et token som er hentet for Azure AD Graph API-er, Outlook API-er eller SharePoint-/OneDrive-API-er, til å kalle opp Microsoft Graph (eller motsatt). Sørg for at ressursen (eller området) appen henter et token for, samsvarer med API-en som appen kaller opp.

**400 Ugyldig forespørsel eller 403 Ingen tilgang: Overholder brukeren organisasjonens policyer for betinget tilgang?**

Basert på policyene for betinget tilgang for en organisasjon kan en bruker som åpner Microsoft Graph-ressurser via appen, bli bedt om ekstra informasjon som ikke finnes i tilgangstokenet som appen opprinnelig hentet. I dette tilfellet mottar appen feilen **400 med *interaction_required*** under henting av tilgangstoken eller feilen **403 med *insufficient_claims*** når Microsoft Graph kalles opp. I begge tilfeller inneholder feilen tilleggsinformasjon som kan presenteres til det autoriserte endepunktet for å be brukeren om mer informasjon (for eksempel godkjenning med flere faktorer eller enhetsregistrering).

Hvis du vil ha mer informasjon om betinget tilgang, kan du se:

- [Håndtere utfordringer med betinget tilgang med MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Utviklerveiledning for betinget tilgang for Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

***Slutt på støtte for Azure Active Directory autentiseringsbibliotek (ADAL) og Azure AD Graph API (AAD Graph)***

- Fra og med 30. juni 2020 kommer vi ikke til å legge til nye funksjoner i godkjenningsbiblioteket for Azure Active Directory (ADAL) og Azure AD Graph-API-en (AAD Graph). Vi vil fortsette å tilby teknisk støtte og sikkerhetsoppdateringer, men vi vil ikke lenger tilby funksjonsoppdateringer.
- Fra og med 30. juni 2022 vil vi avvikle støtten for ADAL og AAD Graph og vil ikke lenger tilby teknisk støtte eller sikkerhetsoppdateringer.
    - Apper som bruker ADAL på eksisterende operativsystemversjoner, vil fortsette å fungere etter dette tidspunktet, men vil ikke få teknisk støtte eller sikkerhetsoppdateringer.
    - Apper som bruker AAD Graph etter dette tidspunktet, vil ikke lenger motta svar fra AAD Graph-endepunktet.

**ADAL-overføring**

Vi anbefaler at du oppdaterer til [Microsofts godkjenningbibliotek (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de nyeste funksjonene og sikkerhetsoppdateringene. Denne anbefalingen gis i forbindelse med at Microsoft overfører programmene sine til MSAL innen fristen for avvikling av kundestøtte. Målet med overføringen av Microsoft-apper til MSAL er å sikre at appene drar nytte av MSALs pågående sikkerhets- og funksjonsforbedringer.

- [Les Vanlige spørsmål om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Finn ut hvordan du overfører apper per plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Hvis du trenger hjelp til å forstå hvilke av appene som bruker ADAL, anbefaler vi at du ser gjennom kildekoden til alle appene, og hvis det er aktuelt, tar du kontakt med en uavhengig programvareleverandør eller appleverandør. Microsoft Kundestøtte kan også gi deg en liste over alle ADAL-appene i tenanten som ikke er fra Microsoft.

**AAD Graph-overføring**

For programmer som bruker AAD Graph, følger du veiledningen for å [overføre Azure AD Graph-apper til Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Sjekklisten for overføring gir et utgangspunkt for å komme i gang](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Appregistreringsportalen for Azure viser hvilke programmer som bruker AAD Graph. Vi anbefaler at du ser gjennom kildekoden for alle appene, og hvis det er aktuelt, tar du kontakt med en uavhengig programvareleverandør eller appleverandør. Microsoft Kundestøtte kan også gi deg informasjon om AAD Graph-bruken i tenanten.

 










