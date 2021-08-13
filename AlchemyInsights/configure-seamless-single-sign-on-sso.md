---
title: Konfigurere sømløs enkel pålogging (SSO)
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
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966046"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Konfigurere sømløs enkel pålogging (SSO)

**Konfigurere programmer**

1. Du bør få verdiene fra programleverandøren. Du kan angi verdiene manuelt eller laste opp en metadatafil for å trekke ut verdien av feltene.
2. Mange apper er allerede forhåndskonfigurert til å fungere med Azure AD. Disse appene er oppført i galleriet med apper som du kan bla gjennom når du legger til en app i Azure AD-tenanten. [Hurtigstartserien](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) tar deg gjennom prosessen.
3. Hvis du vil opprette et program uten galleri, kan du klikke **på + Opprett ditt** eget program-knappen og gi et navn til programmet.
    - Som standard velger den **Integrere andre programmer** du ikke finner i galleriet, som er det riktige alternativet for programmer som ikke er gallerier.
    - Når du har **trykket på Opprett** etter at du har satt inn navnet på programmet, opprettes det et nytt virksomhetsprogram uten galleri.
    - Deretter kan du gå til **Enkel** pålogging **under** Behandle dette programmet, og du vil kunne se ulike teknikker for å implementere det i miljøet.

**Konfigurere Sømløs SSO for et bestemt program**

For appene i galleriet finner du detaljerte, trinnvise instruksjoner. Hvis du vil ha tilgang til trinnene, kan du bla gjennom en liste over alle opplæringer for konfigurasjon av apper i [opplæringsveiledningene for SaaS-appen.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**Konfigurere SAML-basert SSO**

1. [Hurtigstart: Konfigurere SAML-basert](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)enkel pålogging (SSO) for et program i Azure Active Directory (Azure AD) tenant.
2. Hvis du vil lære mer om det SAML-baserte alternativet for enkel pålogging, kan du se [Forstå SAML-basert enkel pålogging](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. Hvis du vil lære om SAML 2.0-godkjenningsforespørsler og svar som Azure Active Directory (Azure AD) støtter for Enkel Sign-On (SSO), kan du se [Enkel Sign-On SAML-protokoll](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Hvis du vil lære hvordan du oppretter og konfigurerer en SAML-basert enkel pålogging (SSO) for programmet i Azure Active Directory (Azure AD) ved hjelp av Microsoft Graph API, kan du se Konfigurere [SAML-basert](https://docs.microsoft.com/graph/application-saml-sso-configure-api)enkel pålogging for programmet ved hjelp av Microsoft Graph API .
5. Hvis du vil lære hvordan Azure AD bruker SAML-protokollen, kan du se Hvordan Microsofts identitetsplattform [bruker SAML-protokollen](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Konfigurere tokener og krav**

1. [Slik tilpasser du krav som er utstedt i SAML-tokenet for bedriftsprogrammer.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Hvis du vil lære hvordan du konfigurerer krav ved hjelp av PowerShell, kan du se Slik tilpasser du krav som sendes inn i tokener for en bestemt app i en [leier (forhåndsvisning).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Hvis du vil lære hvordan du konfigurerer valgfrie krav, kan du se Slik gjør du [det: Oppgi valgfrie krav til appen](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Hvis du vil lære hvordan du bruker attributter for katalogskjemautvidelse til å sende brukerdata til programmer i tokenkrav, kan du se Bruke attributter for [katalogskjemautvidelse i krav](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Hvis du vil lære hvordan du konfigurerer levetid for tokener, kan du se Konfigurerbar levetid for token i Microsofts identitetsplattform [(forhåndsvisning).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Konfigurere policyer for levetid for token (forhåndsvisning)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – I denne artikkelen går vi gjennom et vanlig policyscenario som kan hjelpe deg med å innføre nye regler for tokenlevetid. I eksemplet lærer du hvordan du oppretter en policy som krever at brukere godkjennes oftere i nettappen.

**Feilsøke SSO-konfigurasjon**

- Hvis du vil ha vanlige spørsmål om Azure Active Directory Sømløs enkel Sign-On (sømløs SSO), kan du [Azure Active Directory Problemfri](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)enkel pålogging: Vanlige spørsmål .
- Hvis du vil ha informasjon om feilsøking av vanlige problemer med Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO), kan du se Feilsøke Azure Active Directory [Sømløs enkel pålogging](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
