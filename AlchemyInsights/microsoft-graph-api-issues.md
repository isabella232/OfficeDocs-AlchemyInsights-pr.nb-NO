---
title: Problemer med Microsoft Graph API
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7759"
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975902"
---
# <a name="microsoft-graph-api-issues"></a>Problemer med Microsoft Graph API

Dette emnet kan også gjelde for utviklere som fremdeles bruker Azure AD Graph API. Det anbefales imidlertid på **det sterkeste** at du bruker Microsoft Graph for alle scenarioene for katalog, identitet og tilgangsbehandling.

**Godkjennings- eller godkjenningsproblemer**

- Hvis appen ikke kan hente **tokener** for å ringe Microsoft Graph, velger du Problem med å få et tilgangstoken **(godkjenning)** Microsoft Graph-kategori for å få mer spesifikk hjelp og støtte for dette emnet.
- Hvis appen mottar **401-** eller 403-godkjenningsfeil når du ringer Microsoft Graph, velger du kategorien Får ingen tilgang **(autorisasjon)** Microsoft Graph API for å få mer spesifikk hjelp og støtte for dette emnet.

**Jeg vil bruke Microsoft Graph, men ikke sikker på hvor jeg skal begynne**

- [Oversikt over Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Oversikt over administrasjon av identitet og tilgang i Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Komme i gang med å bygge Microsoft Graph-apper](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – Test Microsoft Graph API-er i leieren eller en demo-tenant

**Jeg vil bruke Microsoft Graph, men støtter det v1.0-katalog-API-ene jeg trenger?**

Microsoft Graph er den anbefalte API-en for katalog-, identitets- og tilgangsbehandling. Det er imidlertid fortsatt noen hull mellom det som er mulig i Azure AD Graph og Microsoft Graph. Se gjennom følgende artikler, som fremhever de mest oppdaterte forskjellene for å hjelpe deg med valget ditt:

- [Forskjeller i ressurstype mellom Azure AD Graph og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Egenskapsforskjeller mellom Azure AD Graph og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Metodeforskjeller mellom Azure AD og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API-en jeg ringer til, fungerer ikke – hvor kan jeg teste mer?**

**Microsoft Graph Explorer** – Test Microsoft Graph API-er i leieren eller en demo-leier, og sjekk også ut eksempelspørringene i Microsoft Graph Explorer. 

**Appen min er for treg og blir også begrensning. Hvilke forbedringer kan jeg gjøre?**

Avhengig av scenarioet ditt finnes det en rekke alternativer du kan bruke for å gjøre programmet mer utførlig, og i noen tilfeller er det mindre utsatt for å bli begrensning av tjenesten (når du foretar for mange anrop).

- [Anbefalte fremgangsmåter for Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Grupperingsforespørsler](https://docs.microsoft.com/graph/json-batching)
- [Spore endringer gjennom deltaspørring](https://docs.microsoft.com/graph/delta-query-overview)
- [Bli varslet om endringer gjennom webhooks](https://docs.microsoft.com/graph/webhooks)
- [Begrensningsveiledning](https://docs.microsoft.com/graph/throttling)

**Hvor finner jeg mer informasjon om feil og kjente problemer?**

- [Microsoft Graph informasjon om feilsvar](https://docs.microsoft.com/graph/errors)
- [Kjente problemer med Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Hvor kan jeg kontrollere statusen for tjenestetilgjengelighet og tilkobling?**

Tjenestetilgjengeligheten og tilkoblingen til de underliggende tjenestene som er tilgjengelige via Microsoft Graph kan påvirke den generelle tilgjengeligheten og ytelsen til Microsoft Graph.

- Hvis Azure Active Directory tjenestetilstand, kan du kontrollere statusen for **sikkerhets- og** identitetstjenester som er oppført på [statussiden for Azure.](https://azure.microsoft.com/status/)
- Hvis Office tjenester som bidrar til Microsoft Graph, kan du kontrollere statusen for tjenestene som er oppført i [Office-instrumentbordet](https://portal.office.com/adminportal/home#/servicehealth)for tjenestetilstand .

Microsoft Graph autorisasjonsfeil kan være et resultat av flere ulike problemer, som de fleste genererer en 401- eller 403-feil. Følgende kan for eksempel føre til autorisasjonsfeil:

- Feil [innhentingsflyter for tilgangstoken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Dårlig konfigurerte [tillatelsesområder](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Mangel på [samtykke](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***Slutt på støtte for Azure Active Directory autentiseringsbibliotek (ADAL) og Azure AD Graph API (AAD Graph)***

**Fra og med 30. juni 2020** legger vi ikke lenger til nye funksjoner i ADAL og Azure AD Graph. Vi vil fortsette å tilby teknisk støtte og sikkerhetsoppdateringer, men vi vil ikke lenger tilby funksjonsoppdateringer.

**Fra og med 30. juni 2022** avslutter vi støtte for ADAL og Azure AD Graph og vil ikke lenger tilby teknisk støtte eller sikkerhetsoppdateringer.

Apper som bruker ADAL på eksisterende OS-versjoner, vil fortsette å fungere etter dette tidspunktet, men vil ikke få teknisk *støtte eller sikkerhetsoppdateringer.*

Apper som bruker Azure AD Graph etter dette tidspunktet, mottar kanskje ikke lenger svar fra Azure AD Graph endepunkt.

**ADAL-overføring**

Vi anbefaler at du oppdaterer til [Microsofts godkjenningbibliotek (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de nyeste funksjonene og sikkerhetsoppdateringene.

Hvis du bruker Microsoft-apper, må du vite at Microsoft er i ferd med å overføre programmene til MSAL innen tidsfristen for kundestøtten utløper, slik at de vil dra nytte av MSALs pågående sikkerhets- og funksjonsforbedringer.

1. [Les Vanlige spørsmål om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Finn ut hvordan du overfører apper per plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Hvis du trenger hjelp til å forstå hvilke av appene som bruker ADAL, anbefaler vi at du går gjennom alle appenes kildekode, og hvis det er aktuelt, kan du ta kontakt med alle LEVERANDØRER eller appleverandører. Microsoft Kundestøtte kan også gi deg en liste over alle ADAL-appene i tenanten som ikke er fra Microsoft.

**AAD Graph-overføring**

For programmer som bruker Azure AD Graph, følger du veiledningen vår for å overføre [Azure AD Graph-apper til Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Sjekklisten for overføring gir et utgangspunkt for å komme i gang](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Appregistreringsportalen for Azure viser hvilke programmer som bruker AAD Graph. Vi anbefaler at du ser gjennom kildekoden for alle appene, og hvis det er aktuelt, tar du kontakt med en uavhengig programvareleverandør eller appleverandør. Microsoft Kundestøtte kan også gi deg en liste over all AAD-Graph bruk i leieren.
3. For at appen skal få tilgang til data i Microsoft Graph, må brukeren eller administratoren gi den de riktige tillatelsene via en samtykkeprosess. Microsoft [Graph-tillatelsesreferansen](https://docs.microsoft.com/graph/permissions-reference) viser tillatelsene som er knyttet til hvert hovedsett av Microsoft Graph API-er. Den gir også veiledning om hvordan du bruker tillatelsene.
