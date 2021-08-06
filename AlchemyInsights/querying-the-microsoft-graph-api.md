---
title: Spørre Microsoft Graph API
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
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923248"
---
# <a name="querying-the-microsoft-graph-api"></a>Spørre Microsoft Graph API

Dette emnet kan også gjelde for utviklere som fremdeles bruker Azure AD Graph API. Det anbefales imidlertid på **det sterkeste** at du bruker Microsoft Graph for alle scenarioene for katalog, identitet og tilgangsbehandling.

**Godkjennings- eller godkjenningsproblemer**

- Hvis appen ikke kan hente **tokener** for å ringe Microsoft Graph, velger du Problem med å få et tilgangstoken **(godkjenning)** Microsoft Graph-kategori for å få mer spesifikk hjelp og støtte for dette emnet.
- Hvis appen mottar **401-** eller 403-godkjenningsfeil når du ringer Microsoft Graph, velger du kategorien Får ingen tilgang **(autorisasjon)** Microsoft Graph API for å få mer spesifikk hjelp og støtte for dette emnet.

**Jeg vil bruke Microsoft Graph, men ikke sikker på hvor jeg skal begynne**

Hvis du vil lære mer om Microsoft Graph, kan du se:

- [Oversikt over Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Oversikt over administrasjon av identitet og tilgang i Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Komme i gang med å bygge Microsoft Graph-apper](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – Test Microsoft Graph API-er i leieren eller en demo-tenant

**Jeg vil bruke Microsoft Graph, men støtter det v1.0-katalog-API-ene jeg trenger?**

Microsoft Graph er den anbefalte API-en for katalog-, identitets- og tilgangsbehandling. Det er imidlertid fortsatt noen hull mellom det som er mulig i Azure AD Graph og Microsoft Graph. Se gjennom følgende artikler, som fremhever de mest oppdaterte forskjellene for å hjelpe deg med valget ditt:

- [Forskjeller i ressurstype mellom Azure AD Graph og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Egenskapsforskjeller mellom Azure AD Graph og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Metodeforskjeller mellom Azure AD og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Når jeg spør *brukerobjektet,* mangler mange av egenskapene**

`GET https://graph.microsoft.com/v1.0/users`returnerer bare 11 egenskaper, siden Microsoft Graph automatisk velger et standardsett med *brukeregenskaper* som skal returneres. Hvis du trenger andre *brukeregenskaper,* kan du $select til å velge egenskapene programmet trenger. Prøv det i **Microsoft Graph Explorer** først.

**Noen brukeregenskapsverdier er *null* selv om jeg vet at de er angitt**

Den mest sannsynlige forklaringen er at programmet har fått *User.ReadBasic.All-tillatelsen.* Dette gjør at programmet kan lese et begrenset sett med brukeregenskaper og returnere alle andre egenskaper som null selv om de er angitt tidligere. Prøv å gi programmet *User.Read.All-tillatelse* i stedet.

Hvis du vil ha mer informasjon, [kan du se Microsoft Graph brukertillatelser](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Jeg har problemer med å bruke OData-spørringsparametere til å filtrere data i forespørslene mine**

Selv om Microsoft Graph støtter en rekke OData-spørringsparametere, støttes mange av disse parameterne ikke fullstendig av katalogtjenester (ressurser som arver fra *directoryObject)* i Microsoft Graph. De samme begrensningene som var til stede i Azure AD Graph for det meste i Microsoft Graph:

1. **Støttes ikke:**$count, $search og $filter *nullverdier* eller *ikke nullverdier*
2. **Støttes ikke:**$filter på bestemte egenskaper (se ressursemner der egenskaper kan filtreres)
3. **Støttes ikke:** sideveksling, filtrering og sortering samtidig
4. **Støttes ikke:** filtrering av en relasjon. For eksempel – finn alle medlemmer av den tekniske gruppen som er i Storbritannia.
5. **Delvis støtte:**$orderby på *bruker* (displayName og userPrincipalName only) og *gruppe*
6. **Delvis** støtte: $filter (støtter bare *eq,* *startswith* *eller* *,* og , og , og begrenset eventuell *)* støtte, $expand (hvis du utvider relasjonene til et enkelt objekt, returneres alle relasjoner, men utvidelse av en samling av objekters relasjoner er begrenset)

Hvis du vil ha mer informasjon, kan [du se Tilpasse svar med spørringsparametere](https://docs.microsoft.com/graph/query-parameters).

**API-en jeg ringer til, fungerer ikke – hvor kan jeg gjøre mer testing?**

**Microsoft Graph Explorer** – Test Microsoft Graph API-er i leieren eller en demo-leier, og sjekk også ut eksempelspørringene i Microsoft Graph Explorer. 

**Når jeg spør etter data, ser det ut som jeg får et ufullstendig datasett tilbake**

Hvis du spør en samling (for eksempel *brukere),* bruker Microsoft Graph sidegrenser på serversiden, slik at resultatene alltid returneres med en standard sidestørrelse. Appen bør alltid forvente å bla gjennom samlinger som returneres fra tjenesten.

Hvis du vil ha mer informasjon, kan du se:

- [Anbefalte fremgangsmåter for Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Sideveksling av Microsoft Graph data i appen](https://docs.microsoft.com/graph/paging)

**Appen min er for treg og blir også begrensning. Hvilke forbedringer kan jeg gjøre?**

Avhengig av scenarioet ditt finnes det en rekke ulike alternativer til din disposisjon for å gjøre programmet mer utførlig, og i noen tilfeller mindre utsatt for å bli begrensning av tjenesten (når du foretar for mange anrop).

Hvis du vil lære mer, kan du se:

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
