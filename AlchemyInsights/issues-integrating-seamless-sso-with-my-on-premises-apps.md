---
title: Problemer med integrering av Sømløs SSO med de lokale appene mine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028301"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemer med integrering av Sømløs SSO med de lokale appene mine

Gjør følgende for å feilsøke problemer med integrering av Sømløs SSO med lokale programmer:

**Anbefalte trinn**

1. Hvis du vil konfigurere **et lokalt program** for enkel pålogging via Programproxy, kan du se Passordhvelv for enkel pålogging [med Programproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting). 
1. **Feilsøke problemer med** programproxy : Vi anbefaler at du begynner med å se gjennom feilsøkingsflyten, Feilsøke problemer med Application Proxy Connector , for å finne ut om Application [Proxy-koblinger](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)er riktig konfigurert. Hvis du fremdeles har problemer med å koble til programmet, følger du feilsøkingstrinnene i Problemer med feilsøking [av programproxyprogram](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Du kan [identifisere CORS-problemer](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) ved hjelp av følgende feilsøkingsverktøy for nettleser:
    1. Start nettleseren, og bla til nettappen.
    1. Trykk **F12 for** å hente frem feilsøkingskonsollen.
    1. Prøv å reprodusere transaksjonen, og se gjennom konsollmeldingen. Et CORS-brudd gir en konsollfeil om opprinnelsen.
    1. Noen CORS-problemer kan ikke løses, for eksempel når appen omdirigerer til login.microsoftonline.com for å godkjenne, og tilgangstokenet utløper. CORS-anropet mislykkes deretter. En midlertidig løsning for dette scenariet er å forlenge levetiden til tilgangstokenet for å hindre at det utløper under en brukers økt. Hvis du vil ha mer informasjon om hvordan du gjør dette, kan du se Konfigurerbar levetid for [token i Microsofts identitetsplattform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Anbefalte dokumenter**

- [Slik konfigurerer du enkel pålogging til et programproxyprogram](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML enkel pålogging for lokale programmer med Programproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Forstå og løse Azure Active Directory cors-problemer med programproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Feilsøke Kerberos begrensede delegeringskonfigurasjoner for programproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)