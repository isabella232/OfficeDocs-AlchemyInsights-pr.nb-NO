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
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012893"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problemer med tokenkrav og attributter

**Oppdatere, konfigurere eller fjerne tokenkrav**

1. Ved å Azure Active Directory (Azure AD), kan du tilpasse kravtypen [for](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) rollekravet i svartokenet som du mottar etter at du har godkjent en app.
2. Programutviklere kan bruke valgfrie krav i Azure AD-programmene til å angi hvilke krav de vil ha i tokener som sendes til programmet. Hvis du vil ha mer informasjon, [kan du se Oppgi valgfrie krav til appen.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Konfigurer gruppekrav for programmer med Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Hvis du bruker Sømløs enkel pålogging i programmet, kan du se Tilpasse krav utstedt i [SAML-tokenet for bedriftsprogrammer](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**Attributttilordning for krav**

1. Hvis du vil konfigurere kravtilordningspolicy ved hjelp av PowerShell, kan du se Tilpasse krav som sendes inn i tokener for en bestemt app i [en leier (forhåndsvisning).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Attributter for katalogskjemautvidelse gjør det mulig å lagre tilleggsdata i Azure Active Directory på brukerobjekter og andre katalogobjekter, for eksempel grupper, leierdetaljer, tjenesteprinsipper. Bare utvidelsesattributter på brukerobjekter kan brukes til å sende ut krav til programmer. [Bruk av attributter for utvidelse av katalogskjema](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) i krav beskriver hvordan du bruker attributter for katalogskjemautvidelse til å sende brukerdata til programmer i tokenkrav.

Hvis du vil ha mer informasjon om tokenkrav, kan du se:

- [Krav i tilgangstokener](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Krav i en id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Krav](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) som du kan forvente i ID-tokener og tilgangstokener utstedt av Azure AD B2C
- [REFERANSE for SAML-tokenkrav](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
