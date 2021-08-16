---
title: Problemer med godkjenningsbiblioteker
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
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028013"
---
# <a name="issues-with-authentication-libraries"></a>Problemer med godkjenningsbiblioteker

1. [Microsofts identitetsplattform-godkjenningsbiblioteker](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) viser Microsoft-støttede og kompatible klient- og mellomvarebiblioteker.
2. Microsoft Authentication Library (MSAL) støtter flere [godkjenningsflyter](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for bruk i ulike programscenarioer.
3. Hvis du vil godkjenne og hente tokener, initialiserer du et nytt offentlig eller konfidensielt klientprogram i koden. Du kan angi flere konfigurasjonsalternativer når du initialiserer klientappen i Microsoft Authentication Library (MSAL). Hvis du vil ha mer informasjon, kan [du se Alternativer for programkonfigurasjon](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Slutt på støtte for Azure Active Directory autentiseringsbibliotek (ADAL) og Azure AD Graph API (AAD Graph)**

**Fra og med 30. juni 2020** legger vi ikke lenger til nye funksjoner i ADAL og Azure AD Graph. Vi vil fortsette å tilby teknisk støtte og sikkerhetsoppdateringer, men vi vil ikke lenger tilby funksjonsoppdateringer.

**Fra og med 30. juni 2022** avslutter vi støtte for ADAL og Azure AD Graph og vil ikke lenger tilby teknisk støtte eller sikkerhetsoppdateringer.

Apper som bruker ADAL på eksisterende OS-versjoner, vil fortsette å fungere etter dette tidspunktet, men vil ikke få teknisk *støtte eller sikkerhetsoppdateringer.*

Apper som bruker Azure AD Graph etter dette tidspunktet, mottar kanskje ikke lenger svar fra Azure AD Graph endepunkt.

**ADAL-overføring**

Vi anbefaler at du oppdaterer til [Microsofts godkjenningbibliotek (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de nyeste funksjonene og sikkerhetsoppdateringene.

Hvis du bruker Microsoft-apper, må du vite at Microsoft er i ferd med å overføre programmene til MSAL innen tidsfristen for kundestøtten utløper, slik at de vil dra nytte av MSAL sine pågående sikkerhets- og funksjonsforbedringer.

Hvis du vil ha mer informasjon, kan du se:

1. [Les Vanlige spørsmål om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Finn ut hvordan du overfører apper per plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Hvis du trenger hjelp til å forstå hvilke av appene som bruker ADAL, anbefaler vi at du går gjennom alle appenes kildekode, og hvis det er aktuelt, kan du ta kontakt med alle LEVERANDØRER eller appleverandører. Microsoft Kundestøtte kan også gi deg en liste over alle ADAL-appene i tenanten som ikke er fra Microsoft.

**AAD Graph-overføring**

For programmer som bruker Azure AD Graph, følger du veiledningen vår for å overføre [Azure AD Graph-apper til Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Sjekklisten for overføring gir deg et poeng for å komme i gang.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Appregistreringsportalen for Azure viser hvilke programmer som bruker AAD Graph. Vi anbefaler at du ser gjennom kildekoden for alle appene, og hvis det er aktuelt, tar du kontakt med en uavhengig programvareleverandør eller appleverandør. Microsoft Kundestøtte kan også gi deg en liste over all AAD-Graph bruk i leieren.
3. For at appen skal få tilgang til data i Microsoft Graph, må brukeren eller administratoren gi den de riktige tillatelsene via en samtykkeprosess. Microsoft [Graph-tillatelsesreferansen](https://docs.microsoft.com/graph/permissions-reference) viser tillatelsene som er knyttet til hvert hovedsett av Microsoft Graph API-er. Den gir også veiledning om hvordan du bruker tillatelsene.
