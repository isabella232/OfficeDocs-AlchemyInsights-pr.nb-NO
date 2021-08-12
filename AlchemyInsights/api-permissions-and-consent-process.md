---
title: API-tillatelser og samtykkeprosess
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932070"
---
# <a name="api-permissions-and-consent-process"></a>API-tillatelser og samtykkeprosess

For at appen skal få tilgang til data i Microsoft Graph, må brukeren eller administratoren gi den de riktige tillatelsene via en samtykkeprosess. [Microsoft Graph-tillatelsesreferanse](https://docs.microsoft.com/graph/permissions-reference) viser tillatelsene som er knyttet til hvert hovedsett av Microsoft Graph API-er. Den gir også veiledning om hvordan du bruker tillatelsene.

**Konfigurere eller oppdatere tjenesteprinsipp**

- [Opprett serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – Denne artikkelen viser deg hvordan du oppretter et nytt servicePrincipal-objekt.
- Opprett en [Azure AD-app](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) &-tjenesteprinsipp i portalen – Denne artikkelen viser deg hvordan du oppretter et nytt Azure Active Directory-program (Azure AD)-program og tjenesteprinsipp som kan brukes med den rollebaserte tilgangskontrollen.
- [Apper &](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) tjenesteprinsipper i Azure AD – Denne artikkelen beskriver programregistrering, programobjekter og tjenesteprinsipper i Azure Active Directory: hva de er, hvordan de brukes og hvordan de er relatert til hverandre.

**Legge til eller oppdatere appregistrering og gi administratorsamtykke**

- [Opprette en appregistrering](https://docs.microsoft.com/graph/api/application-post-applications) – Denne artikkelen viser deg hvordan du oppretter et nytt programobjekt.
- [Oppdatere en appregistrering – API-tillatelser](https://docs.microsoft.com/graph/api/application-update) – Denne artikkelen viser deg hvordan du oppdaterer egenskapene for et programobjekt.
- [Gi administratorsamtykke](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) – For administratorsamtykke og samtykke generelt krever vi at en administrator eksplisitt gir samtykke.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – Beholder for rollebehandling for enhetlige rolledefinisjoner og rolletilordninger for Microsoft 365 RBAC-leverandører som støtter flere hovedstoler og flere omfang i én enkelt rolletilordning. Dette er forskjellig fra *ressurstypen rbacApplication.* Microsoft Intune er et eksempel på en slik RBAC-leverandør. En rolletilordning i Intune kan ha en matrise med hovedstoler og en rekke omfangsgrupper. **Dette er i betaversjon, noe som betyr at det fortsatt er under utvikling og ikke anbefalt for bruk i produksjon.**
