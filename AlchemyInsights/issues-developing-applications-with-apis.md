---
title: Problemer med å utvikle programmer med APIer
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
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975024"
---
# <a name="issues-developing-applications-with-apis"></a>Problemer med å utvikle programmer med APIer

Hvis du vil begynne å bruke Azure Active Directory Graph API, kan du se hurtigst [Art veiledning for Azure ad Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) eller vise den [interaktive referanse dokumentasjonen for Azure ad Graph API](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Slutten av støtte for Azure Active Directory Authentication Library (ADAL) og Azure AD Graph API (AAD-graf)**

**Fra og med 30. juni 2020** vil vi ikke lenger legge til nye funksjoner i ADAL og Azure ad Graph. Vi vil fortsette å gi tekniske støtte og sikkerhets oppdateringer, men vil ikke lenger gi funksjons oppdateringer.

**Fra og med 30. juni 2022** vil vi avslutte støtte for ADAL og Azure ad Graph og vil ikke lenger gi tekniske støtte eller sikkerhets oppdateringer.

Apper som bruker ADAL på eksisterende OS-versjoner vil fortsatt fungere etter denne tiden, men får ingen tekniske støtte eller sikkerhets oppdateringer.

Apper som bruker Azure AD Graph etter dette tidspunktet, vil kanskje ikke lenger motta svar fra Azure AD Graph-endepunktet.

**ADAL overføring**

Vi anbefaler at du oppdaterer til [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de nyeste funksjonene og sikkerhets oppdateringene.

Hvis du bruker Microsoft-apper, vet du at Microsoft er i ferd med å overføre sine programmer til MSAL med tids fristen for slutt på støtte, slik at de kommer til å dra nytte av MSALs kontinuerlige sikkerhets-og funksjons forbedringer.

1. [Les ADAL vanlige spørsmål](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Lær om hvordan du overfører apper på hver enkelt plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Hvis du trenger hjelp til å forstå hvilke av appene som bruker ADAL, anbefaler vi at du ser gjennom alle programmenes kilde kode, og hvis det er aktuelt, kan du nå ut til alle uavhengige program vare leverandører. Microsoft kunde støtte kan også gi deg en liste over alle ikke-Microsoft-ADAL-apper i leieren din.

**Overføring av AAD-graf**

For programmer som bruker Azure AD Graph, følger du veiledningen vår for å overføre [apper i Azure ad Graph til Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Overførings sjekk listen vår gir et komme i gang-punkt](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Registrerings portalen for Azure-apper viser hvilke programmer som bruker AAD-graf. Vi anbefaler at du ser gjennom alle appenes kilde kode, og hvis det er aktuelt, kan du nå ut til alle uavhengige program vare leverandører. Microsoft kunde støtte kan også gi deg en liste over all bruk av AAD-graf i leieren din.
1. Brukeren eller administratoren må gi den riktige tillatelsene via en samtykke prosess for at appen skal få tilgang til data i Microsoft Graph. [Referansen Microsoft Graph-tillatelser](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) viser tillatelsene som er tilknyttet hvert hoved sett med Microsoft Graph-APIer. Den gir deg også veiledning om hvordan du bruker tillatelsene.
