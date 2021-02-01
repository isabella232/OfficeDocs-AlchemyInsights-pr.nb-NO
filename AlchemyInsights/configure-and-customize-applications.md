---
title: Konfigurere og tilpasse programmer
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
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063660"
---
# <a name="configure-and-customize-applications"></a>Konfigurere og tilpasse programmer

**Konfigurere programmer**

1. [Hurtigstart: Konfigurer egenskaper for](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) et program i Azure Active Directory-leieren (Azure AD) viser deg hvordan du konfigurerer noen av egenskapene for en app.
2. For å integrere programmene dine med Azure Active Directory har vi utviklet en samling av veiledninger [som](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) veileder deg gjennom konfigurasjonen.
3. [Hvordan du konfigurerer et programproxyprogram](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) hjelper deg med å forstå hvordan du konfigurerer et programproxyprogram i Azure AD, slik at de lokale programmene vises i skyen.
4. [Last ned PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)og konfigurer programmet: Følg instruksjonene i Konfigurere *PingAccess for Azure AD for* å beskytte programmer som er publisert ved hjelp av Microsoft Azure AD-programproxy på nettstedet ping-identitet, og last ned den nyeste versjonen av PingAccess.

**Feilkonfigurert program (AADSTS650056)**

1. Kontroller at du har tilgang til programmet fra påloggingsadressen du har fått av eieren av programmet. Ellers må du logge på programmet gjennom den normale prosessen. I de fleste tilfeller løses dette automatisk på en naturlig måte. Hvis den ikke gjør det, kan dette innlegget hjelpe deg med å feilsøke og løse det.
2. **Hvis organisasjonen din eier programmet** (det vil si at programregistreringen er i organisasjonen):
    - Vi anbefaler som et minimum at eller `User.Read` `openid` delegert tillatelse fra **Microsoft Graph** legges til.
    - Kontroller at programmet og alle tillatelsene er samtykket til. Du kan kontrollere dette ved å se på **Status-kolonnen** for programregistreringen i **API-tillatelser.**
    - I noen tilfeller kan programmet være tredjeparts, men det kan være registrert i organisasjonen. Bekreft om dette programmet er oppført i appregistreringene (Ikke Enterprise-programmer).
    - Hvis du fortsatt ser denne feilmeldingen. Deretter må du kanskje bygge nettadressen for samtykke som **beskrives i trinn 4.**
3. **Hvis organisasjonen ikke er eieren av programmet og bruker det som et tredjepartsprogram:**
    - Hvis du er global administrator/firmaadministrator, skal du se samtykkeskjermen. Kontroller at du merker av for Samtykke på vegne **av organisasjonen.**
    - Hvis du ikke ser samtykkeskjermen, sletter du Enterprise-programmet og prøver på nytt.
    - Hvis du fortsatt ser denne feilmeldingen. Deretter må du kanskje bygge nettadressen for samtykke som **beskrives i trinn 4.**
4. Bygg nettadressen som skal brukes med samtykke: Hvis programmet er utformet for å få tilgang til en bestemt ressurs, kan det hende du ikke kan bruke samtykkeknappene fra Azure Portal, må du manuelt generere din egen samtykke-nettadresse og bruke denne.
    - Du må hente og fra eieren `{App-Id}` `{App-Uri-Id}` av programmet. `{Tenant-Id}` blir tenantidentifikatoren din. Dette vil være eller `yourdomain.onmicrosoft.com` katalog-ID-en din.
    - Hvis programmet har tilgang til seg selv for ressursen, er `{App-Id}` og vil være det `{App-Uri-Id}` samme.
5. Hvis du vil ha mer informasjon, kan du se Problemer med å logge [på SAML-baserte, konfigurerte apper for enkel pålogging.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Tilpasse programmer**

- Legg til varemerking på organisasjonens påloggingsside [for Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) – Bruk organisasjonens logo og egendefinerte fargevalg for å gi et konsekvent utseende og en konsekvent følelse av påloggingssidene for Azure Active Directory (Azure AD).
- [Legg til det egendefinerte domenenavnet ved hjelp av Azure Active Directory-portalen.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) Hver nye Azure AD-leier leveres med et opprinnelig domenenavn. Du kan ikke endre eller slette det opprinnelige domenenavnet, men du kan legge til organisasjonens navn. Ved å legge til egendefinerte domenenavn kan du opprette brukernavn som er kjente for brukerne.
