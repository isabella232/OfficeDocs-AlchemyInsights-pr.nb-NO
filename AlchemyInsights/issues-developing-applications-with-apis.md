---
title: Problemer med å utvikle programmer med API-er
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
- "9004343"
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013469"
---
# <a name="issues-developing-applications-with-apis"></a>Problemer med å utvikle programmer med API-er

Hvis du vil begynne å bruke Azure Active Directory Graph API, kan du se hurtigstartveiledningen [for Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) eller vise den interaktive referansedokumentasjonen for [Azure AD Graph API](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Slutt på støtte for Azure Active Directory autentiseringsbibliotek (ADAL) og Azure AD Graph API (AAD Graph)**

**Fra og med 30. juni 2020** legger vi ikke lenger til nye funksjoner i ADAL og Azure AD Graph. Vi vil fortsette å tilby teknisk støtte og sikkerhetsoppdateringer, men vi vil ikke lenger tilby funksjonsoppdateringer.

**Fra og med 30. juni 2022** avslutter vi støtte for ADAL og Azure AD Graph og vil ikke lenger tilby teknisk støtte eller sikkerhetsoppdateringer.

Apper som bruker ADAL på eksisterende operativsystemversjoner, vil fortsette å fungere etter dette tidspunktet, men vil ikke få teknisk støtte eller sikkerhetsoppdateringer.

Apper som bruker Azure AD Graph etter dette tidspunktet, mottar kanskje ikke lenger svar fra Azure AD Graph endepunkt.

**ADAL-overføring**

Vi anbefaler at du oppdaterer til [Microsofts godkjenningbibliotek (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de nyeste funksjonene og sikkerhetsoppdateringene.

Hvis du bruker Microsoft-apper, må du vite at Microsoft er i ferd med å overføre programmene til MSAL innen tidsfristen for kundestøtten utløper, slik at de vil dra nytte av MSAL sine pågående sikkerhets- og funksjonsforbedringer.

1. [Les vanlige spørsmål om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Lær om hvordan du overfører apper per plattform.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Hvis du trenger hjelp til å forstå hvilke av appene som bruker ADAL, anbefaler vi at du går gjennom alle appenes kildekode, og hvis det er aktuelt, kan du ta kontakt med alle LEVERANDØRER eller appleverandører. Microsoft Kundestøtte kan også gi deg en liste over alle ADAL-appene i tenanten som ikke er fra Microsoft.

**AAD Graph-overføring**

For programmer som bruker Azure AD Graph, følger du veiledningen vår for å overføre [Azure AD Graph-apper til Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Sjekklisten for overføring gir et utgangspunkt for å komme i gang](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Appregistreringsportalen for Azure viser hvilke programmer som bruker AAD Graph. Vi anbefaler at du ser gjennom kildekoden for alle appene, og hvis det er aktuelt, tar du kontakt med en uavhengig programvareleverandør eller appleverandør. Microsoft Kundestøtte kan også gi deg en liste over all AAD-Graph bruk i leieren.
1. For at appen skal få tilgang til data i Microsoft Graph, må brukeren eller administratoren gi den de riktige tillatelsene via en samtykkeprosess. Microsoft [Graph-tillatelsesreferansen](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) viser tillatelsene som er knyttet til hvert hovedsett av Microsoft Graph API-er. Den gir også veiledning om hvordan du bruker tillatelsene.
