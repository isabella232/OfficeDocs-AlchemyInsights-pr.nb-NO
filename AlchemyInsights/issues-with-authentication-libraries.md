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
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063639"
---
# <a name="issues-with-authentication-libraries"></a>Problemer med godkjenningsbiblioteker

1. [Biblioteker for Godkjenning av Microsoft-identitetsplattform](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) viser biblioteker for Microsoft-støttede og kompatible klienter og middleware.
2. Microsoft Authentication Library (MSAL) støtter flere [godkjenningsflyter](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for bruk i ulike programscenarier.
3. Hvis du vil godkjenne og skaffe tokener, initialiserer du et nytt offentlig eller konfidensielt klientprogram i koden. Du kan angi flere konfigurasjonsalternativer når du initialiserer klientappen i Microsoft Authentication Library (MSAL). Hvis du vil ha mer informasjon, kan du [se konfigurasjonsalternativer for programmet.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Slutt på støtte for Azure Active Directory Authentication Library (ADAL) og Azure AD Graph API (AAD Graph)**

**Fra og med 30. juni 2020** vil vi ikke lenger legge til nye funksjoner i ADAL og Azure AD Graph. Vi vil fortsette å tilby teknisk støtte og sikkerhetsoppdateringer, men vi vil ikke lenger tilby funksjonsoppdateringer.

**Fra og med 30. juni 2022** avslutter vi støtten for ADAL og Azure AD Graph og vil ikke lenger tilby teknisk støtte eller sikkerhetsoppdateringer.

Apper som bruker ADAL på eksisterende OS-versjoner, vil fortsette å fungere etter dette tid, men vil ikke få noen teknisk støtte *eller sikkerhetsoppdateringer.*

Apper som bruker Azure AD Graph etter dette tid, kan ikke lenger motta svar fra Azure AD Graph-endepunktet.

**ADAL-overføring**

Vi anbefaler at du oppdaterer til [Microsofts godkjenningbibliotek (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de nyeste funksjonene og sikkerhetsoppdateringene.

Hvis du bruker Microsoft-apper, må du vite at Microsoft er i ferd med å overføre programmene til MSAL innen tidsfristen for slutten av støtten, slik at de vil dra nytte av MSALs pågående sikkerhets- og funksjonsforbedringer.

Hvis du vil ha mer informasjon, kan du se:

1. [Les Vanlige spørsmål om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Finn ut hvordan du overfører apper per plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Hvis du trenger hjelp til å forstå hvilke apper som bruker ADAL, anbefaler vi at du går gjennom alle appenes kildekode, og hvis aktuelt, kan du ta kontakt med eventuelle ISV-er eller appleverandører. Microsoft Kundestøtte kan også gi deg en liste over alle ADAL-appene i tenanten som ikke er fra Microsoft.

**AAD Graph-overføring**

For programmer som bruker Azure AD Graph, følger du veiledningen vår for [å overføre Azure AD Graph-apper til Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Sjekklisten for overføring gir deg et komme i gang-punkt.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Appregistreringsportalen for Azure viser hvilke programmer som bruker AAD Graph. Vi anbefaler at du ser gjennom kildekoden for alle appene, og hvis det er aktuelt, tar du kontakt med en uavhengig programvareleverandør eller appleverandør. Microsoft Kundestøtte kan også gi deg en liste over all AAD Graph-bruk i tenanten din.
3. Brukeren eller administratoren må gi appen de riktige tillatelsene via en samtykkeprosess for at den skal få tilgang til data i Microsoft Graph. [Tillatelsesreferansen for Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) viser tillatelsene som er knyttet til hvert hovedsett av Microsoft Graph API-er. Den gir også veiledning om hvordan du bruker tillatelsene.
