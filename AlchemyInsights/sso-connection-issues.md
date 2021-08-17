---
title: SSO-tilkoblingsproblemer
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
- "9004357"
- "7810"
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084355"
---
# <a name="sso-connection-issues"></a>SSO-tilkoblingsproblemer

1. Følg [hurtiginnføringen: Konfigurere egenskaper for en programveiledning](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) for å konfigurere programmet.
2. Avhengig av programmet og alternativet [for enkel](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) pålogging du velger, følger du den aktuelle veiledningen nedenfor:
    - Hvis du vil konfigurere **et lokalt program** for **SAML-basert** enkel pålogging, kan du se SAML enkel pålogging for lokale programmer [med Programproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - Hvis du vil konfigurere **et skyprogram** for **passordbasert enkel** pålogging, kan du se  [Konfigurere enkel pålogging med passord](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - Hvis du vil konfigurere **et lokalt program** for enkel pålogging via Programproxy, kan du se Passordhvelv for enkel pålogging [med Programproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting). 
3. **Feilsøke problemer med** programproxy : Vi anbefaler at du begynner med å se gjennom feilsøkingsflyten, Feilsøke problemer med Application Proxy Connector , for å finne ut om Application [Proxy-koblinger](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)er riktig konfigurert. Hvis du fremdeles har problemer med å koble til programmet, følger du feilsøkingsflyten i Problemer med feilsøking [av programproxyprogrammet](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Du kan [identifisere CORS-problemer](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) ved hjelp av feilsøkingsverktøy i nettleseren:
    - Start nettleseren, og bla til nettappen.
    - Trykk **F12 for** å hente frem feilsøkingskonsollen.
    - Prøv å reprodusere transaksjonen, og se gjennom konsollmeldingen. Et CORS-brudd gir en konsollfeil om opprinnelsen.
    - Noen CORS-problemer kan ikke løses, for eksempel når appen omdirigerer til login.microsoft.com for å godkjenne, og tilgangstokenet utløper. CORS-anropet mislykkes deretter. En midlertidig løsning for dette scenariet er å forlenge levetiden til tilgangstokenet for å hindre at det utløper under en brukers økt. Hvis du vil ha mer informasjon om hvordan du gjør dette, kan du se Konfigurerbar levetid for [token i Microsofts identitetsplattform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. **Feilsøke SAML-basert** enkel pålogging: Vi anbefaler at du kontrollerer Problemer med å logge på [SAML-baserte](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)apper for enkel pålogging, for å finne løsningene på problemene du mest sannsynlig vil støte på.
5. **Feilsøking av passordbasert** enkel pålogging : Vi anbefaler at du kontrollerer Feilsøke passordbasert enkel pålogging i [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)for å finne løsningene på problemene du mest sannsynlig vil støte på.
6. Hvis du vil ha tilkoblingsproblemer mens du bruker et VPN, kan du se Slik bruker du enkel pålogging [(SSO) over VPN og Wi-Fi tilkoblinger](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
