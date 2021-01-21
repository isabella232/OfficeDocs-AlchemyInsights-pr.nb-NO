---
title: Problemer med tokener
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917039"
---
# <a name="issues-with-tokens"></a>Problemer med tokener

Du kan bruke følgende Fremgangs måte for å behandle problemer som er knyttet til spesial tegn:

1. Du kan angi leve tiden til en Access-, ID-eller SAML-token utstedt av Microsoft Identity Platform. Du kan angi token-levetid for alle apper i organisasjonen, for et multi-leier (multi-Organization) program eller for en bestemt tjeneste konto i organisasjonen. Hvis du vil ha mer informasjon, kan du se [konfigurerbare token-levetid i Microsoft Identity Platform (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Access-tokener gjør det mulig for klienter å ringe beskyttede nett-APIer, og brukes av nett-APIer til å utføre godkjenning og autorisasjon. I henhold til OAuth-spesifikasjonen er tilgangs koder ugjennomsiktige strenger uten et angitt format-noen identitets leverandører (IDPs) bruk guider, andre bruker krypterte BLOBer. Microsoft Identity Platform bruker en rekke formater for tilgangstoken, avhengig av konfigurasjonen av APIEN som godtar tokenet. Hvis du vil vite hvordan APIEN kan validere og bruke kravene i et tilgangstoken, kan du se [Microsoft Identity Platform Access tokens](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. Microsoft Authentication Library (MSAL) støtter flere godkjennings flyter for bruk i ulike program scenarioer. Hvis du vil ha mer informasjon, kan du se [godkjennings flyter](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. Tilordningen av OAuth 2,0-Autorisasjons koden kan brukes i apper som er installert på en enhet for å få tilgang til beskyttede ressurser, for eksempel nett-APIer. Ved hjelp av Microsoft Identity Platform-implementeringen av OAuth 2,0, kan du legge til påloggings-og API-tilgang til mobil-og skrive bords programmer. Se [Microsoft Identity Platform and OAuth 2,0 Authorization Code Flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) for hvordan du skal programmere direkte mot protokollen i programmet, ved hjelp av et hvilket som helst språk.
5. OpenID Connect (OIDC) er en godkjennings protokoll som er bygd på OAuth 2,0, som du kan bruke til å logge på en bruker i et program på en sikker måte. Når du bruker Microsoft Identity Platform Endpoint ' s-implementeringen av OpenID Connect, kan du legge til påloggings-og API-tilgang i appene dine. [Microsoft Identity Platform and OpenID Connect Protocol](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) viser hvordan du gjør dette uavhengig av språk og beskriver hvordan du sender og mottar http-meldinger uten å bruke Microsoft Open-Source-biblioteker.
    - UserInfo-endepunktet er en del av OIDC-standarden, utformet for å returnere krav om brukeren som godkjennes. Hvis du vil ha mer informasjon, kan du se [Microsoft Identity Platform UserInfo Endpoint](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - Et nett BAS- [API-anrop i en nett App ved hjelp av Azure ad og OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) -eksempel viser hvordan du bygger et MVC-nettprogram som bruker Azure ad for pålogging ved hjelp av OpenID Connect-protokollen, og deretter kan du ringe til en nett BAS-API under den påloggede brukerens identitet ved hjelp av tokener som ble skaffet via OAuth 2,0. Dette eksemplet bruker OpenID koble ASP .net OWIN mellomvare og ADAL .net.
6. [Konfigurere et program til å eksponere en nett](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) BAS-API – i denne hurtigst Art kassen registrerer du en nett BAS-API med Microsoft Identity Platform og eksponerer den til klient programmer ved å legge til et eksempel område. Ved å registrere nett-API-en og eksponere den gjennom omfang, kan du gi tillatelses BAS ert tilgang til ressursene til autoriserte brukere og klient programmer som får tilgang til API-en.
7. I Azure Active Directory B2C (Azure AD B2C)-flyt for ressurs eier passord legitimasjon (ROPC) er en OAuth-standard godkjennings flyt. I denne flyten kan et program, også kalt den beroende parten, utveksle gyldig legitimasjon for tokener. Legitimasjonen inneholder en bruker-ID og et passord. De returnerte tokenene er et ID-token, tilgangstoken og et refresh-token. Hvis du vil ha mer informasjon, kan du se [konfigurere passord for en ressurs eier legitimasjons flyt i Azure Active Directory-B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

