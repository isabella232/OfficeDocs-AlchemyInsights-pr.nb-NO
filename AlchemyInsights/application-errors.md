---
title: Program feil
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
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984584"
---
# <a name="application-errors"></a>Program feil

Leter du etter informasjon om **AADSTS-feilkodene** som returneres fra Azure Active Directory (STS) for sikkerhets kode (Azure ad)? Les [Azure ad-godkjenning og feil koder for godkjenning](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) for å finne AADSTS feil beskrivelser, løsninger og noen foreslåtte løsninger.

Godkjennings feil kan være et resultat av flere forskjellige problemer, som oftest genererer en 401-eller 403-feil. Følgende kan for eksempel føre til godkjennings feil:

- Feil [innhentings flyt for token](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) for tilgangstoken 
- Dårlig konfigurerte [tillatelses omfang](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Mangel på [samtykke](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Hvis du vil løse vanlige godkjennings feil, kan du prøve Fremgangs måten nedenfor som Sams varer best med feilen du mottar. Mer enn én kan påløpe.

**401 uautorisert feil melding: er tokenet ditt gyldig?**

Kontroller at programmet presenterer et gyldig tilgangstoken til Microsoft Graph som en del av forespørselen. Denne feilen betyr ofte at tilgangstoken kan mangle i forespørsels hodet for HTTP-godkjenning, eller at tokenet er ugyldig eller er utløpt. Vi anbefaler på det sterkeste at du bruker [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) for å få tilgang til token-innhenting. I tillegg kan denne feilen oppstå hvis du prøver å bruke et delegert tilgangstoken som er gitt til en personlig Microsoft-konto, for å få tilgang til en API som bare støtter jobb-eller skole kontoer (organisasjons kontoer).

**403 forbudt-feil: har du valgt riktig tillatelses sett?**

Kontroller at du har bedt om det riktige tillatelses settet basert på Microsoft Graph-APIene som programmet ringer til. Du finner anbefalte minimums tillatelser i alle Microsoft Graph API Reference Method-emner. I tillegg må disse tillatelsene gis til programmet av en bruker eller administrator. Tildeling av tillatelser skjer vanligvis gjennom en samtykke side eller ved å gi tillatelser ved hjelp av registrerings blad for Azure Portal-programmet. Klikk **nødvendige tillatelser** fra **Innstillinger** -blad for programmet, og klikk deretter **gi tillatelser**.

- [Microsoft Graph-tillatelser](https://docs.microsoft.com/graph/permissions-reference) 
- [Lære om Azure AD-tillatelser og samtykke](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 forbudt-feil: ble appen hentet et token for å samsvare med valgte tillatelser?**

Kontroller at typen tillatelser som er forespurt eller innvilget, Sams varer med typen tilgangs kode som appen henter. Du ber kanskje om å gi program tillatelser, men bruker delegerte interaktive Code Flow-tokener i stedet for klient legitimasjons flyt tokener, eller ber om og gir delegert tillatelse, men bruker tokener for klient legitimasjons flyt i stedet for delegerte kode flyt tegn.

- [Få tilgang på vegne av brukere og Delegerte tillatelser](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v 2.0-OAuth 2,0 Autorisasjons kode flyt](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Få tilgang uten en User (Daemon-tjeneste) og program tillatelser](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v 2.0 – OAuth 2,0 klient legitimasjons flyt](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 forbudt-feil: tilbakestille passordet**

For øyeblikket er det ingen tillatelse for tjeneste-til-tjeneste-Daemon for program tillatelse som tillater tilbakestilling av bruker passord. Disse APIene støttes bare ved hjelp av den interaktive delegerte koden som flyter med en pålogget administrator.

- [Microsoft Graph-tillatelser](https://docs.microsoft.com/graph/permissions-reference)

**403 forbudt: har brukeren tilgang og er de lisensiert?**

For delegert kode flyter evalueres Microsoft Graph hvis forespørselen er tillatt basert på tillatelsene som er gitt til appen, og tillatelsene som den påloggede brukeren har. Vanligvis indikerer denne feilen at brukeren ikke er privilegert nok til å utføre forespørselen, eller fordi brukeren ikke er lisensiert for dataene du har tilgang til. Bare brukere med de nødvendige tillatelsene eller lisensene kan gjøre forespørselen utført.

**403 forbudt: har du valgt riktig ressurs-API?**

API-tjenester som Microsoft Graph Kontroller at AUD-krav (mål gruppe) i den mottatte tilgangs koden Sams varer med verdien den forventer for seg selv, og hvis den ikke er det, fører det til en 403 forbudt feil. En vanlig feil som resulterer i denne feilen, prøver å bruke et token som skaffes for Azure AD Graph-APIer, Outlook-APIer eller SharePoint/OneDrive-APIer for å ringe Microsoft Graph (eller omvendt). Kontroller at ressursen (eller omfanget) som programmet ditt henter et token for, Sams varer med APIEN som appen ringer.

**400 Ugyldig forespørsel eller 403 forbudt: bruker brukeren til å overholde organisasjonens policyer for betinget tilgang (CA)?**

På grunnlag av organisasjonens sertifiserings instans policyer kan en bruker som har tilgang til Microsoft Graph-ressurser via appen, være Challenged for ytterligere informasjon som ikke finnes i tilgangstoken som programmet opprinnelig anskaffet. I dette tilfellet mottar appen en 400 med en *interaction_required* -feil under token-innhenting eller en 403 med *insufficient_claims* feil når du ringer til Microsoft Graph. I begge tilfeller inneholder feil svaret tilleggs informasjon som kan presenteres for godkjennings ende punktet for å være en utfordring for brukeren om tilleggs informasjon (for eksempel godkjenning av flere faktorer eller enhets registrering).

- [Behandling av betingede tilgang ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Veiledning for utvikler for Azure Active Directory betinget tilgang](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
