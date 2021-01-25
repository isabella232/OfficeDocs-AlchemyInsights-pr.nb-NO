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
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974761"
---
# <a name="issues-developing-applications"></a>Problemer med å utvikle programmer

Hvis du vil feilsøke de vanligste problemene ved bygging av Azure Active Directory-apper (AD), kan du se følgende artikler:

- [Jeg har problemer med å logge deg på programmet (ene) ved bruk av Chrome-leser](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Jeg vet ikke hvordan du endrer standard verdien for leve tiden for token for programmet](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Jeg er forvirret om hvordan program samtykke fungerer](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Jeg vet ikke hvordan jeg gir tillatelser til programmet mitt](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Jeg forstår ikke forskjellen mellom delegerte og applikasjons tillatelser](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Slutten av støtte for Azure Active Directory Authentication Library (ADAL) og Azure ad Graph API (AAD-graf)** _

- Fra og med 30. juni 2020 vil vi ikke lenger legge til nye funksjoner i Azure Active Directory Authentication Library (ADAL) og Azure AD Graph API (AAD-graf). Vi vil fortsette å gi tekniske støtte og sikkerhets oppdateringer, men vil ikke lenger gi funksjons oppdateringer.

- Fra og med 30. juni 2022 vil vi avslutte støtte for ADAL og AAD-graf og vil ikke lenger gi tekniske støtte eller sikkerhets oppdateringer. Som følge av denne situasjonen er følgende implikasjoner:

    - Apper som bruker ADAL på eksisterende OS-versjoner vil fortsatt fungere etter denne tiden, men får ingen tekniske støtte eller sikkerhets oppdateringer.

    - Apper som bruker AAD Graph etter dette tidspunktet vil kanskje ikke lenger motta svar fra ende punktet til AAD-Graph

_ *ADAL-overføring**

Hvis du bruker Microsoft-apper, anbefaler vi at du oppdaterer til Microsoft Authentication Library (MSAL), som har de nyeste funksjonene og sikkerhets oppdateringene. Denne anbefalingen er i konteksten til Microsoft som starter prosessen med å overføre sine apper til MSAL av tids fristen for slutt på støtte. 

Overføringen av Microsoft-appene til MSAL sikrer at appene drar nytte av MSALs kontinuerlige sikkerhets-og funksjons forbedringer.

1. [Les ADAL vanlige spørsmål](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Lær om hvordan du overfører apper på en per-plattform-basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Hvis du trenger hjelp til å forstå hvilke av appene dine som bruker ADAL, anbefaler vi at du ser gjennom alle appenes kilde kode og, hvis det er aktuelt, nå ut til alle uavhengige program vare leverandører (ISV-er) eller program leverandører. Microsoft kunde støtte kan også gi deg en liste over alle ikke-Microsoft-ADAL-apper i leieren din.

**Overføring av AAD-graf**

For programmer som bruker AAD-grafen, følger du veiledningen vår for å overføre apper for AAD-graf til Microsoft Graph:

1. [Overførings sjekk listen vår gir et komme i gang-punkt](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Registrerings portalen for Azure-apper viser hvilke programmer som bruker AAD-graf. Vi anbefaler at du ser gjennom alle appenes kilde kode, og når det er aktuelt, nå til alle uavhengige program vare leverandører (ISV) eller program leverandører. Microsoft kunde støtte kan også gi deg informasjon om AAD Graph-bruk i leieren din.







