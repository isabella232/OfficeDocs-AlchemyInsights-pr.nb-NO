---
title: Spørre etter Microsoft Graph API
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
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974424"
---
# <a name="querying-the-microsoft-graph-api"></a>Spørre etter Microsoft Graph API

Dette emnet kan også gjelde for utviklere som fremdeles bruker Azure AD Graph API. Det anbefales imidlertid på det **sterkeste** at du bruker Microsoft Graph for alle dine katalog-, identitets-og tilgangs behandlings scenarioer.

**Problemer med godkjenning eller autorisasjon**

- Hvis appen **ikke kan hente tokener** for å ringe Microsoft Graph, velger du **problem med å få en tilgangs kode (Authentication)** Microsoft Graph-kategori for å få mer spesifikk hjelp og støtte på dette emnet.
- Hvis appen **mottar godkjennings feil for 401 eller 403** når du ringer til Microsoft Graph, velger du avmerkings boksen få tilgang til å få **tilgangen nektes (godkjenning)** Microsoft Graph API-kategori for å få mer spesifikk hjelp og støtte på dette emnet.

**Jeg vil bruke Microsoft Graph, men ikke sikker på hvor du skal begynne**

Hvis du vil lære mer om Microsoft Graph, kan du se:

- [Oversikt over Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Oversikt over identitets-og tilgangs behandling i Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Komme i gang med å bygge Microsoft Graph-apper](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – test Microsoft Graph-APIer i leieren eller en demonstrasjons leier

**Jeg vil bruke Microsoft Graph, men har den støtte for v 1.0-katalog-APIene jeg trenger?**

Microsoft Graph er den anbefalte APIEN for katalog, identitet og tilgangs behandling. Det finnes imidlertid fremdeles noen tomrom mellom hva som er mulig i Azure AD Graph og Microsoft Graph. Se gjennom følgende artikler, som uthever de mest oppdaterte forskjellene for å hjelpe deg med det du velger:

- [Ressurs type forskjeller mellom Azure AD Graph og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Egenskaps forskjeller mellom Azure AD Graph og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Metode forskjeller mellom Azure AD og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Når jeg spør etter *bruker* objektet, mangler mange av egenskapene**

`GET https://graph.microsoft.com/v1.0/users` returnerer bare 11 egenskaper, som Microsoft Graph automatisk velger et standard sett med *bruker* egenskaper som skal returneres. Hvis du trenger andre *bruker* egenskaper, kan du bruke $SELECT til å velge hvilke egenskaper programmet trenger. Prøv det i **Microsoft Graph Explorer** først.

**Noen bruker egenskaps verdier er *null* selv om at de er angitt**

Den mest sannsynlige forklaringen er at programmet har fått tillatelsen *User. ReadBasic. all* -tillatelse. Dette gjør at programmet kan lese et begrenset sett med bruker egenskaper, og returnere alle andre egenskaper som null selv om de er angitt tidligere. Prøv å gi program *brukeren. read. all* -tilgang i stedet.

Hvis du vil ha mer informasjon, kan du se [bruker tillatelser for Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Jeg har problemer med å bruke spørrings parametere for OData til å filtrere data i mine forespørsler**

Selv om Microsoft Graph støtter en rekke spørrings parametere for OData, støttes ikke mange av disse parameterne fullt ut av katalog tjenester (ressurser som arver fra *directoryObject*) i Microsoft Graph. De samme begrensningene som fantes i Azure AD Graph, vedvarer for den meste parten i Microsoft Graph:

1. **Støttes ikke**: $count, $search og $filter på *null* eller *not null* -verdier
2. **Støttes ikke**: $filter på bestemte egenskaper (se ressurs emner som kan filtreres på)
3. **Støttes ikke**: side veksling, filtrering og sortering på samme tid
4. **Støttes ikke**: filtrere på en relasjon. For eksempel finner du alle medlemmer av gruppen ingeniør som er i Storbritannia.
5. **Delvis støtte**: $OrderBy på *bruker* (bare DisplayName og userPrincipalName) og *gruppe*
6. **Del støtte**: $filter (støtter bare *EQ*, *startswith* *eller* *, og* *begrenset)* støtte, $Expand (utvidelse av ett objekts relasjoner returnerer alle relasjoner, men å utvide en samling av objekt relasjoner er begrenset)

Hvis du vil ha mer informasjon, kan du se [tilpasse svar med spørrings parametere](https://docs.microsoft.com/graph/query-parameters).

**APIEN jeg ringer til, fungerer ikke – hvor kan jeg gjøre flere tester?**

**Microsoft Graph Explorer** – test Microsoft Graph-APIene i leieren eller en demonstrasjons leier, og sjekk ut **utvalgs spørringene** i Microsoft Graph Explorer.

**Når jeg spør etter data det ser ut til at jeg får et ufullstendig data sett tilbake**

Hvis du spør på en samling (for eksempel *brukere*), bruker Microsoft Graph side grenser for serverside, slik at resultatene alltid returneres med en standard side størrelse. Appen skal alltid vente på å bla gjennom samlinger som returneres fra tjenesten.

Hvis du vil ha mer informasjon, kan du se:

- [Beste Fremgangs måter i Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Bla etter Microsoft Graph-data i appen](https://docs.microsoft.com/graph/paging)

**Appen min er for langsomt og blir også begrenset. Hvilke forbedringer kan jeg gjøre?**

Avhengig av scenariet, er det en rekke forskjellige alternativer for avhending for å gjøre programmet mer utført, og i noen tilfeller mindre utsatt for at du blir begrenset av tjenesten (når du foretar for mange samtaler).

Hvis du vil lære mer, kan du se:

- [Beste Fremgangs måter i Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Satsvise forespørsler](https://docs.microsoft.com/graph/json-batching)
- [Spore endringer gjennom en delta-spørring](https://docs.microsoft.com/graph/delta-query-overview)
- [Få beskjed om endringer via webhooks](https://docs.microsoft.com/graph/webhooks)
- [Begrensende veiledning](https://docs.microsoft.com/graph/throttling)

**Hvor kan jeg finne mer informasjon om feil og kjente problemer?**

- [Feil svar informasjon for Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Kjente problemer med Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Hvor kan jeg sjekke status for tjeneste tilgjengelighet og tilkobling?**

Tjeneste tilgjengeligheten og tilkoblingen til de underliggende tjenestene som du kan få tilgang til gjennom Microsoft Graph, kan påvirke den generelle tilgjengeligheten og ytelsen til Microsoft Graph.

- For tjeneste tilstanden Azure Active Directory kan du kontrollere statusen for **sikkerhets-og identitets** tjenester som er oppført på [status siden for Azure](https://azure.microsoft.com/status/).
- For Office-tjenester som bidrar til Microsoft Graph, må du kontrollere statusen for tjenestene som er oppført i [instrument bordet for tilstands tilstand for Office Service](https://portal.office.com/adminportal/home#/servicehealth).
