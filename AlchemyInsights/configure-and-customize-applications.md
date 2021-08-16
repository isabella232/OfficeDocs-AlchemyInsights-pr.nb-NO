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
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044997"
---
# <a name="configure-and-customize-applications"></a>Konfigurere og tilpasse programmer

**Konfigurere programmer**

1. Hurtigstart: Konfigurere egenskaper for et program i [Azure Active Directory (Azure AD) tenanten](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) viser deg hvordan du konfigurerer noen av egenskapene for en app.
2. For å bidra til å integrere programmene med Azure Active Directory, har vi utviklet en samling med [veiledninger](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) som veileder deg gjennom konfigurasjonen.
3. [Slik konfigurerer du et program for](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) programproxy hjelper deg med å forstå hvordan du konfigurerer et Programproxy-program i Azure AD for å vise de lokale programmene i skyen.
4. [Last ned PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)og konfigurer programmet: Følg instruksjonene i Konfigurere *PingAccess for Azure AD for* å beskytte programmer som er publisert ved hjelp av Microsoft Azure AD-programproxyen på pingidentitetsnettstedet, og last ned den nyeste versjonen av PingAccess.

**Feilkonfigurerte programfeil (AADSTS650056)**

1. Kontroller at du får tilgang til programmet fra påloggingsadressen som er angitt av programeieren. Ellers må du logge på programmet gjennom den normale prosessen. I de fleste tilfeller vil dette automatisk løses på en naturlig måte. Hvis det ikke gjør det, kan dette innlegget hjelpe deg med å feilsøke og løse det.
2. **Hvis organisasjonen eier programmet (det** vil si at programregistreringen er i organisasjonen):
    - Vi anbefaler at eller delegert tillatelse fra `User.Read` `openid` Microsoft **Graph** er lagt til.
    - Kontroller at programmet og alle tillatelsene er samtykket til. Du kan bekrefte dette ved å se på **Status-kolonnen** i programregistreringen i **API-tillatelser**.
    - I enkelte scenarioer kan programmet være tredjeparts, men det kan være registrert i organisasjonen. Bekreft om dette programmet er oppført i appregistreringene (ikke enterprise-programmer).
    - Hvis du fortsatt ser denne feilmeldingen. Deretter må du kanskje bygge nettadressen for samtykke som er beskrevet i **trinn 4.**
3. **Hvis organisasjonen ikke er programeier og bruker det** som et tredjepartsprogram:
    - Hvis du er global/firmaadministrator, skal du se samtykkeskjermen. Kontroller at du merker av for **Samtykke på vegne av organisasjonen.**
    - Hvis du ikke ser samtykkeskjermen, sletter du Enterprise-programmet og prøver på nytt.
    - Hvis du fortsatt ser denne feilmeldingen. Deretter må du kanskje bygge nettadressen for samtykke som er beskrevet i **trinn 4.**
4. Bygg nettadressen for samtykke manuelt som skal **brukes:** Hvis programmet er utformet for å få tilgang til en bestemt ressurs, kan det hende du ikke kan bruke Samtykke-knappene fra Azure-portalen, må du manuelt generere din egen nettadresse for samtykke og bruke dette.
    - Du må få og fra `{App-Id}` `{App-Uri-Id}` eieren av programmet. `{Tenant-Id}` vil være tenantidentifikatoren din. Dette vil enten være `yourdomain.onmicrosoft.com` eller katalog-ID-en.
    - Hvis programmet får tilgang til seg selv for ressursen, vil `{App-Id}` og `{App-Uri-Id}` være det samme.
5. Hvis du vil ha mer informasjon, kan du se Problemer med å [logge på SAML-baserte apper](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)for enkel pålogging.

**Tilpasse programmer**

- Legg til varemerking på organisasjonens [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) påloggingsside – Bruk organisasjonens logo og egendefinerte fargevalg for å gi en konsekvent utseende og egenskap på påloggingssidene for Azure Active Directory (Azure AD).
- [Legg til det egendefinerte domenenavnet](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) ved hjelp av Azure Active Directory portalen – Alle nye Azure AD-leiere leveres med et opprinnelig domenenavn. Du kan ikke endre eller slette det opprinnelige domenenavnet, men du kan legge til organisasjonens navn. Når du legger til egendefinerte domenenavn, kan du opprette brukernavn som er kjente for brukerne.
