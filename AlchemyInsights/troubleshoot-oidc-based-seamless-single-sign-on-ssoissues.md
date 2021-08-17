---
title: Feilsøke problemer med OIDC-basert sømløs enkel pålogging (SSO)
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
- "9004357"
- "9375"
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105787"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Feilsøke problemer med OIDC-basert sømløs enkel pålogging (SSO)

- Hvis du vil lære hvordan du legger til en OIDC-basert app i Azure-leieren, kan du se [Hurtigstart: Konfigurere OIDC-basert](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)enkel pålogging (SSO) for et program i Azure Active Directory -leieren (Azure AD).
- Hvis du vil ha mer informasjon om apper som bruker OpenID-Koble til til å implementere enkel pålogging, kan du se [Forstå OIDC-basert](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)enkel pålogging .
- Hvis du vil ha informasjon i tilfelle du velger å skrive koden ved å sende og behandle HTTP-forespørsler direkte eller bruke et tredjeparts open-source-bibliotek, i stedet for å bruke et av våre open source-biblioteker, kan du se [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)og OpenID Koble til-protokoller på Microsofts identitetsplattform .

**Protokoller**

1. Microsofts identitetsplattform og [implisitt](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) tilskuddsflyt – Den definerende egenskap ved det implisitte tilskuddet er at tokener (ID-tokener eller tilgangstokener) returneres direkte fra /authorize-endepunktet i stedet for /token-endepunktet. Dette brukes ofte som en del av autorisasjonskodeflyten, i det som kalles hybridflyten – henting av **ID-tokenet på /authorize-forespørselen** sammen med en autorisasjonskode . Denne artikkelen beskriver hvordan du programmerer direkte mot protokollen i programmet for å be om tokener fra Azure AD.
2. Microsofts identitetsplattform og [OAuth 2.0-autorisasjonskodeflyt](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – autorisasjonskodetildelingen OAuth 2.0 kan brukes i apper som er installert på en enhet for å få tilgang til beskyttede ressurser, for eksempel nett-API-er. Ved hjelp Microsofts identitetsplattform av OAuth 2.0 kan du legge til pålogging og API-tilgang til **mobil- og skrivebordsappene.** Denne artikkelen beskriver hvordan du programmerer direkte mot protokollen i programmet ved hjelp av et hvilket som helst språk.
3. [Microsofts identitetsplattform og OpenID Koble til-protokollen](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – Når du bruker Microsofts identitetsplattform implementeringen av OpenID Koble til, kan du legge til påloggings- og API-tilgang til appene. Denne artikkelen viser hvordan du gjør dette uavhengig av språk og beskriver hvordan du sender og mottar HTTP-meldinger uten å bruke **microsoft-biblioteker med åpen kilde.**
4. Microsofts identitetsplattform og [OAuth 2.0-klientlegitimasjonsflyten](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – Du kan bruke OAuth 2.0-klientlegitimasjonen som er angitt i RFC 6749, også kalt **tobente OAuth**, for å få tilgang til nettbaserte ressurser ved hjelp av identiteten til et program. Denne typen tilskudd brukes vanligvis for server-til-server-samhandlinger som må kjøre i bakgrunnen, uten umiddelbar samhandling med en bruker. Disse typene programmer kalles ofte **daemoner eller** **tjenestekontoer.** Denne artikkelen beskriver hvordan du programmerer direkte mot protokollen i programmet.
