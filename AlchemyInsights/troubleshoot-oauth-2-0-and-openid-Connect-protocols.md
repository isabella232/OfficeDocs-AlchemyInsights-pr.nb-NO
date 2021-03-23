---
title: Feilsøke OAuth 2.0- og OpenID Connect-protokoller
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036402"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Feilsøke OAuth 2.0- og OpenID Connect-protokoller

Hvis du vil løse problemer med OAuth 2.0 og OpenID Connect, utfører du følgende anbefalte trinn:

Se følgende artikler som er relatert til konfigurasjon og feilsøking av OAuth 2.0- og OpenID Connect-protokoller:

- Microsofts identitetsplattform og [OAuth 2.0-autorisasjonskodeflyt](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – Denne artikkelen beskriver hvordan du programmerer direkte mot kodetildelingsflyten **(PKCE)** i programmet ved hjelp av et hvilket som helst språk.
- [Microsofts identitetsplattform og OAuth 2.0-klientlegitimasjonsflyt](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – Denne artikkelen beskriver hvordan du programmerer direkte mot klientlegitimasjonsflyten i programmet. 
- [Microsofts identitetsplattform og OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) Passordlegitimasjon for ressurseier – Denne artikkelen beskriver hvordan du programmerer direkte mot **ROPC-flyten** i programmet.
    - Microsofts identitetsplattform støtter bare ROPC for Azure AD-tenanter, og ikke for personlige kontoer. Dette betyr at du må bruke et leier-spesifikt endepunkt **https://login.microsoftonline.com/{TenantId_or_Name}) (** eller **organisasjonens** endepunkt.
    - Personlige kontoer som er invitert til en Azure AD-tenant, kan ikke bruke ROPC.
    - Kontoer som ikke har passord, kan ikke logge på via ROPC. I dette scenariet anbefaler vi at du bruker en annen flyt for appen i stedet.
    - Hvis brukere må bruke godkjenning med flere faktorer [(MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) til å logge på programmet, blokkeres de.
    - ROPC støttes ikke i scenarioer for [hybrid identitetsforbund](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) (for eksempel Azure AD og ADFS som brukes til å godkjenne lokale kontoer). Hvis brukere blir omdirigert til en lokal identitetsleverandør, kan ikke Azure AD teste brukernavnet og passordet mot denne identitetsleverandøren. [Pass-through-godkjenning](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) støttes imidlertid med ROPC.
    - Et unntak fra et scenario med hybrid identitetsforbund vil være følgende: Home Realm Discovery-policy med **AllowCloudPasswordValidation** satt til **TRUE,** vil gjøre det mulig for ROPC-flyt å fungere for brukere i forbund når det lokale passordet synkroniseres til skyen. Hvis du vil ha mer informasjon, kan du se Aktivere [direkte ROPC-godkjenning av brukere](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) i forbund for eldre programmer 
- Microsofts identitetsplattform og [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) På vegne av flyt – Denne artikkelen beskriver hvordan du programmerer direkte mot **OBO-flyten på** vegne av programmet.
- [Microsofts](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) identitetsplattform og OpenID Connect-protokoll – Denne artikkelen viser hvordan du implementerer OpenID Connect-protokollen uavhengig av språk, og beskriver hvordan du sender og mottar HTTP-meldinger uten å bruke microsoft-biblioteker med åpen kilde.

**Access-tokener**

[Tilgangstokener for Microsoft-identitetsplattform](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Finn ut hvordan API-en kan validere og bruke påstandene i et tilgangstoken. All dokumentasjon i denne artikkelen, unntatt der det er notert, gjelder bare for tokener utstedt for API-er du har registrert. Det gjelder ikke tokener utstedt for Microsoft-eide API-er, og disse tokenene kan heller ikke brukes til å validere hvordan Microsoft-identitetsplattformen vil utstede tokener for en API du oppretter.

**Programkonfigurasjon**

[Omdiriger URI-restriksjoner](https://docs.microsoft.com/azure/active-directory/develop/reply-url) og begrensninger for URI (svaradresse) – Lær hvordan du konfigurerer URI-en for omadressering (svar-URL). En omdirigerings-URI eller svar-URL-adresse er plasseringen der autorisasjonsserveren sender brukeren når appen har blitt godkjent og gitt en autorisasjonskode eller tilgangstoken. Autorisasjonsserveren sender koden eller tokenet til URI-en for omdirigering. Så det er viktig at du registrerer riktig plassering som en del av registreringsprosessen for appen.

**Klargjøring av program**

[Opplæring: Utvikle og planlegge klargjøring for](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) et SCIM-endepunkt – Denne artikkelen beskriver hvordan du bygger et SCIM-endepunkt og integrerer med AAD-klargjøringstjenesten.


