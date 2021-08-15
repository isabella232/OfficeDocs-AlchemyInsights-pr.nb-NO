---
title: Problemer med å utvikle programmer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013433"
---
# <a name="issues-developing-applications"></a>Problemer med å utvikle programmer

Hvis du vil feilsøke de vanligste problemene når du Azure Active Directory (AD)-apper, kan du se følgende artikler:

- [Jeg ser problemer med å logge på program(er) bare ved hjelp av Chrome-nettleseren](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Jeg vet ikke hvordan jeg endrer standardverdiene for tokenlevetid for programmet](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Jeg er forvirret over hvordan programsamtykke fungerer](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Jeg vet ikke hvordan jeg gir tillatelser til programmet mitt](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Jeg forstår ikke forskjellen mellom delegerte tillatelser og programtillatelser](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Slutt på støtte for Azure Active Directory autentiseringsbibliotek (ADAL) og Azure AD Graph API (AAD Graph)***

- Fra og med 30. juni 2020 kommer vi ikke til å legge til nye funksjoner i godkjenningsbiblioteket for Azure Active Directory (ADAL) og Azure AD Graph-API-en (AAD Graph). Vi vil fortsette å tilby teknisk støtte og sikkerhetsoppdateringer, men vi vil ikke lenger tilby funksjonsoppdateringer.

- Fra og med 30. juni 2022 vil vi avvikle støtten for ADAL og AAD Graph og vil ikke lenger tilby teknisk støtte eller sikkerhetsoppdateringer. Som et resultat av denne betingelsen er følgende konsekvenser:

    - Apper som bruker ADAL på eksisterende operativsystemversjoner, vil fortsette å fungere etter dette tidspunktet, men vil ikke få teknisk støtte eller sikkerhetsoppdateringer.

    - Apper som bruker AAD Graph etter dette tidspunktet, kan ikke lenger motta svar fra AAD-Graph endepunktet

**ADAL-overføring**

Hvis du bruker Microsoft-apper, anbefaler vi å oppdatere til Microsoft Authentication Library (MSAL), som har de nyeste funksjonene og sikkerhetsoppdateringene. Denne anbefalingen er i sammenheng med at Microsoft starter prosessen med å overføre appene til MSAL innen tidsfristen for slutten av støtten. 

Overføringen av Microsofts apper til MSAL sikrer at appene drar nytte av MSALs pågående sikkerhets- og funksjonsforbedringer.

1. [Les Vanlige spørsmål om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Finn ut hvordan du overfører apper per plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Hvis du trenger hjelp til å forstå hvilke av appene som bruker ADAL, anbefaler vi at du går gjennom alle appenes kildekode, og eventuelt kan ta kontakt med uavhengige programvareleverandører eller appleverandører. Microsoft Kundestøtte kan også gi deg en liste over alle ADAL-appene i tenanten som ikke er fra Microsoft.

**AAD Graph-overføring**

For programmer som bruker AAD Graph, følger du veiledningen vår for å overføre AAD Graph-apper til Microsoft Graph:

1. [Sjekklisten for overføring gir et utgangspunkt for å komme i gang](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Appregistreringsportalen for Azure viser hvilke programmer som bruker AAD Graph. Vi anbefaler at du går gjennom kildekoden til alle appene dine, og hvis det er aktuelt, kan du ta kontakt med uavhengige programvareleverandører eller appleverandører. Microsoft Kundestøtte kan også gi deg informasjon om AAD Graph bruk i leieren.







