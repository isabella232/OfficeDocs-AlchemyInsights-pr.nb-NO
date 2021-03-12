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
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714154"
---
# <a name="microsoft-graph-api-issues"></a>Problemer med Microsoft Graph API

Dette emnet kan også gjelde for utviklere som fremdeles bruker Azure AD Graph API. Det anbefales imidlertid på **det sterkeste** at du bruker Microsoft Graph for alle scenariene for katalog-, identitets- og tilgangsbehandling.

**Godkjennings- eller godkjenningsproblemer**

- Hvis appen ikke kan skaffe **tokener** til å ringe Microsoft Graph, kan du velge Problem med å få et tilgangstoken **(godkjenning)** Microsoft Graph-kategori for å få mer spesifikk hjelp og støtte for dette emnet.
- Hvis appen mottar **401-** eller 403-godkjenningsfeil når du ringer Microsoft Graph, kan du velge feilmeldingen Får ingen tilgang **(Authorization)** Microsoft Graph API for å få mer spesifikk hjelp og støtte for dette emnet.

**Jeg vil bruke Microsoft Graph, men er ikke sikker på hvor jeg skal begynne**

- [Oversikt over Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Oversikt over identitets- og tilgangsbehandling i Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Komme i gang med å bygge Microsoft Graph-apper](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – test Microsoft Graph API-er i tenanten din eller en demo-tenant

**Jeg vil bruke Microsoft Graph, men støtter det API-ene for v1.0-katalogen jeg trenger?**

Microsoft Graph er det anbefalte API-et for katalog-, identitets- og tilgangsbehandling. Det er imidlertid fortsatt noen hull mellom det som er mulig i Azure AD Graph og Microsoft Graph. Se gjennom følgende artikler, som fremhever de mest oppdaterte forskjellene som kan hjelpe deg med valget ditt:

- [Forskjeller på ressurstypen mellom Azure AD Graph og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Egenskapsforskjeller mellom Azure AD Graph og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Metodeforskjeller mellom Azure AD og Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API-en jeg ringer, fungerer ikke – hvor kan jeg teste mer?**

**Microsoft Graph Explorer** – test Microsoft Graph API-er i tenanten din eller en demo-leier, og sjekk også ut eksempelspørringene **i** Microsoft Graph Explorer.

**Appen min er for treg og blir også begrensning. Hvilke forbedringer kan jeg gjøre?**

Avhengig av scenarioet finnes det en rekke alternativer du kan velge mellom for å gjøre programmet mer velfellerende, og i noen tilfeller mindre utsatt for å bli begrensning av tjenesten (når du foretar for mange anrop).

- [Anbefalte fremgangsmåter for Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Grupperingsforespørsler](https://docs.microsoft.com/graph/json-batching)
- [Spore endringer gjennom delta-spørring](https://docs.microsoft.com/graph/delta-query-overview)
- [Bli varslet om endringer via webhooks](https://docs.microsoft.com/graph/webhooks)
- [Begrensningsveiledning](https://docs.microsoft.com/graph/throttling)

**Hvor finner jeg mer informasjon om feil og kjente problemer?**

- [Informasjon om feilsvar i Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Kjente problemer med Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Hvor kan jeg kontrollere statusen for tjenestetilgjengelighet og tilkobling?**

Tjenestetilgjengeligheten og tilkoblingen til de underliggende tjenestene som kan nås via Microsoft Graph, kan påvirke den generelle tilgjengeligheten og ytelsen til Microsoft Graph.

- For tjenestetilstand for Azure Active Directory kontrollerer du statusen for **tjenester for** sikkerhet og identitet som er oppført på [statussiden for Azure.](https://azure.microsoft.com/status/)
- Når det gjelder Office-tjenester som bidrar til Microsoft Graph, kan du kontrollere statusen for tjenester som er oppført i instrumentbordet for [tjenestetilstand.](https://portal.office.com/adminportal/home#/servicehealth)

Godkjenningsfeil i Microsoft Graph kan skyldes flere forskjellige problemer, og de fleste genererer en 401- eller 403-feil. Følgende kan for eksempel føre til autorisasjonsfeil:

- Feil [innhentingsflyter for tilgangstoken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Dårlig konfigurerte [tillatelsesområder](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Mangel på [samtykke](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Avvikling av kundestøtte for godkjenningsbiblioteket for Azure Active Directory (ADAL) og Azure AD Graph-API-en (AAD Graph)_* _

_*Fra og med 30. juni 2020**, vil vi ikke lenger legge til nye funksjoner i ADAL og Azure AD Graph. Vi vil fortsette å tilby teknisk støtte og sikkerhetsoppdateringer, men vi vil ikke lenger tilby funksjonsoppdateringer.

**Fra og med 30. juni 2022** avslutter vi støtten for ADAL og Azure AD Graph og vil ikke lenger tilby teknisk støtte eller sikkerhetsoppdateringer.

Apper som bruker ADAL på eksisterende OS-versjoner, vil fortsette å fungere etter dette tid, men vil ikke få noen teknisk støtte *eller sikkerhetsoppdateringer.*

Apper som bruker Azure AD Graph etter dette tid, kan ikke lenger motta svar fra Azure AD Graph-endepunktet.

**ADAL-overføring**

Vi anbefaler at du oppdaterer til [Microsofts godkjenningbibliotek (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de nyeste funksjonene og sikkerhetsoppdateringene.

Hvis du bruker Microsoft-apper, må du vite at Microsoft er i ferd med å overføre programmene til MSAL innen tidsfristen for slutten av støtten, slik at de vil dra nytte av MSALs pågående sikkerhets- og funksjonsforbedringer.

1. [Les Vanlige spørsmål om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Finn ut hvordan du overfører apper per plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Hvis du trenger hjelp til å forstå hvilke apper som bruker ADAL, anbefaler vi at du går gjennom alle appenes kildekode, og hvis aktuelt, kan du ta kontakt med eventuelle ISV-er eller appleverandører. Microsoft Kundestøtte kan også gi deg en liste over alle ADAL-appene i tenanten som ikke er fra Microsoft.

**AAD Graph-overføring**

For programmer som bruker Azure AD Graph, følger du veiledningen vår for [å overføre Azure AD Graph-apper til Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Sjekklisten for overføring gir et utgangspunkt for å komme i gang](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Appregistreringsportalen for Azure viser hvilke programmer som bruker AAD Graph. Vi anbefaler at du ser gjennom kildekoden for alle appene, og hvis det er aktuelt, tar du kontakt med en uavhengig programvareleverandør eller appleverandør. Microsoft Kundestøtte kan også gi deg en liste over all AAD Graph-bruk i tenanten din.
3. Brukeren eller administratoren må gi appen de riktige tillatelsene via en samtykkeprosess for at appen skal få tilgang til data i Microsoft Graph. [Tillatelsesreferansen for Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) viser tillatelsene som er knyttet til hvert hovedsett av Microsoft Graph API-er. Den gir også veiledning om hvordan du bruker tillatelsene.
