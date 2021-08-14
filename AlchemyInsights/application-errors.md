---
title: Programfeil
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931458"
---
# <a name="application-errors"></a>Programfeil

Leter du etter informasjon om **AADSTS-feilkodene** som returneres fra sikkerhetstokentjenesten for Azure Active Directory (Azure AD)? Les [Azure AD-godkjenning og](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) autorisasjonsfeilkoder for å finne AADSTS-feilbeskrivelser, løsninger og noen foreslåtte midlertidige løsninger.

Autorisasjonsfeil kan være et resultat av flere ulike problemer. De fleste av disse genererer en 401- eller 403-feil. Følgende kan for eksempel føre til autorisasjonsfeil:

- Feil [innhentingsflyter for tilgangstoken](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Dårlig konfigurerte [tillatelsesområder](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Mangel på [samtykke](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Hvis du vil løse vanlige autorisasjonsfeil, kan du prøve fremgangsmåten nedenfor som samsvarer best med feilen du mottar. Mer enn ett kan gjelde.

**Feil 401 Uautorisert: Er tokenet gyldig?**

Kontroller at programmet presenterer et gyldig tilgangstoken til Microsoft Graph som en del av forespørselen. Denne feilen betyr ofte at tilgangstokenet mangler i forespørselshodet for HTTP-godkjenning, eller at tokenet er ugyldig eller utløpt. Vi anbefaler på det sterkeste at du bruker [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) for tilgangstokenanskaffelse. I tillegg kan denne feilen oppstå hvis du prøver å bruke et delegert tilgangstoken gitt til en personlig Microsoft-konto for å få tilgang til en API som bare støtter jobb- eller skolekontoer (organisasjonskontoer).

**Feil 403 Ingen tilgang: Har du valgt riktig sett med tillatelser?**

Kontroller at du har bedt om riktig sett med tillatelser basert på Microsoft Graph API-ene appanropene dine. Anbefalte minst privilegerte tillatelser gis i alle referansemetodeemnene for Microsoft Graph API. I tillegg må disse tillatelsene gis til programmet av en bruker eller administrator. Tildeling av tillatelser skjer vanligvis via en samtykkeside eller ved å gi tillatelser ved hjelp av registreringsbladet for Azure Portal-programmet. Gå til **Innstillinger**-bladet til programmet, klikk på **Nødvendige tillatelser**, og klikk deretter på **Gi tillatelser**.

- [Microsoft Graph-tillatelser](https://docs.microsoft.com/graph/permissions-reference) 
- [Forstå tillatelse og samtykke for Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**Feil 403 Ingen tilgang: Hentet appen et token for å samsvare med valgte tillatelser?**

Kontroller at typen tillatelser som er forespurt eller gitt, samsvarer med typen tilgangstoken som appen skaffer. Du kan be om og gi programtillatelser, men bruke delegerte interaktive kodeflyttokener i stedet for tokener for klientlegitimasjonsflyt, eller be om og gi delegerte tillatelser, men bruke tokener for klientlegitimasjonsflyt i stedet for tokener for delegert kodeflyt.

- [Få tilgang på vegne av brukere og delegerte tillatelser](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 – OAuth 2.0-autorisasjonskodeflyt](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Få tilgang uten en bruker (daemon-tjeneste) og programtillatelser](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 – OAuth 2.0-klientlegitimasjonsflyt](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**Feil 403 Ingen tilgang: Tilbakestilling av passord**

Det er for øyeblikket ingen daemon-tjeneste-til-tjeneste-tillatelser som tillater tilbakestilling av brukerpassord. Disse API-ene støttes bare ved bruk av de interaktive delegerte kodeflytene med en pålogget administrator.

- [Microsoft Graph-tillatelser](https://docs.microsoft.com/graph/permissions-reference)

**403 Ingen tilgang: Har brukeren tilgang og lisens?**

For delegerte kodeflyter evaluerer Microsoft Graph om forespørselen er tillatt basert på tillatelsene som er gitt til appen, og tillatelsene som den påloggede brukeren har. Generelt sett indikerer denne feilen at brukeren ikke har nok rettigheter til å utføre forespørselen, eller brukeren er ikke lisensiert for tilgang til dataene. Bare brukere med nødvendige tillatelser eller lisenser kan utføre forespørselen.

**403 Ingen tilgang: Valgte du riktig ressurs-API?**

API-tjenester som Microsoft Graph kontrollere at aud-kravet (målgruppen) i det mottatte tilgangstokenet samsvarer med verdien den forventer for seg selv, og hvis ikke, resulterer det i en 403 Forbudt feil. En vanlig feil som fører til i denne feilen, er å prøve å bruke et token som er hentet for Azure AD Graph API-er, Outlook API-er eller SharePoint-/OneDrive-API-er, til å kalle opp Microsoft Graph (eller motsatt). Sørg for at ressursen (eller området) appen henter et token for, samsvarer med API-en som appen kaller opp.

**400 Ugyldig forespørsel eller 403 Ingen tilgang: Overholder brukeren organisasjonens policyer for betinget tilgang?**

Basert på organisasjonens CA-policyer kan en bruker som har tilgang til Microsoft Graph-ressurser via appen, bli utfordret for tilleggsinformasjon som ikke finnes i tilgangstokenet appen opprinnelig anskaffet. I dette tilfellet mottar appen feilen 400 med *interaction_required* under henting av tilgangstoken eller feilen 403 med *insufficient_claims* når Microsoft Graph kalles opp. I begge tilfeller inneholder feilsvaret tilleggsinformasjon som kan presenteres for det autoriserte endepunktet for å utfordre brukeren for tilleggsinformasjon (for eksempel godkjenning med flere faktorer eller registrering av enheter).

- [Håndtere betingede tilgangsutfordringer ved hjelp av MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Utviklerveiledning for betinget tilgang for Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
