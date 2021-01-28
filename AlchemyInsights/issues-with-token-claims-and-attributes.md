---
title: Problemer med tokenkrav og attributter
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035967"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problemer med tokenkrav og attributter

**Oppdatere, konfigurere eller fjerne tokenkrav**

1. Ved å bruke Azure Active Directory (Azure AD) kan du tilpasse kravtypen [for](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) rollekravet i svartokenet som du mottar etter at du har godkjent en app.
2. Programutviklere kan bruke valgfrie krav i Azure AD-programmene til å angi hvilke krav de ønsker i tokener som sendes til deres program. Hvis du vil ha mer informasjon, [kan du se Oppgi valgfrie krav til appen.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Konfigurer gruppekrav for programmer med Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)
4. Hvis du bruker sømløs enkel pålogging i programmet, kan du se tilpasse krav utstedt i [SAML-token for bedriftsprogrammer.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Attributttilordning for krav**

1. Hvis du vil konfigurere policy for kravtilordning ved hjelp av PowerShell, kan du se Tilpasse krav som sendes inn tokener for en bestemt app i [en leier (forhåndsvisning).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Attributter for katalogskjemautvidelse gjør det mulig å lagre tilleggsdata i Azure Active Directory på brukerobjekter og andre katalogobjekter, for eksempel grupper, leierdetaljer, tjenesteprinsipper. Bare utvidelsesattributter på brukerobjekter kan brukes for å sende krav til programmer. [Bruk av attributter for katalogskjemautvidelse](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) i krav beskriver hvordan du bruker attributter for katalogskjemautvidelse til å sende brukerdata til programmer i tokenkrav.

Hvis du vil ha mer informasjon om tokenkrav, kan du se:

- [Krav i tilgangstoken](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Krav i en id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Krav](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) som du kan forvente i ID-tokener og tilgangstokener utstedt av Azure AD B2C
- [Referanse for SAML-tokenkrav](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
