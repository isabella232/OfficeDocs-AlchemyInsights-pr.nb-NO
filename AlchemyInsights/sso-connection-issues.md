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
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935154"
---
# <a name="sso-connection-issues"></a>SSO-tilkoblingsproblemer

1. Følg [hurtigveiledningen: Konfigurere egenskaper for en programveiledning](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) for å konfigurere programmet.
2. Avhengig av programmet og alternativet [for enkel](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) pålogging du velger, følger du riktig veiledning nedenfor:
    - Hvis du vil **konfigurere et** lokalt program for **SAML-basert** enkel pålogging, kan du se SAML enkel pålogging for lokale programmer [med programproxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - Hvis du vil **konfigurere et skyprogram** for **passordbasert** enkel pålogging, kan du se [Konfigurere enkel pålogging for passord.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Hvis du vil konfigurere **et lokalt program** for enkel pålogging via programproxy, kan du se Passordhvelv for enkel pålogging med [programproxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) 
3. **Feilsøking av problemer** med programproxy: Vi [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)anbefaler at du starter med å se gjennom feilsøkingsflyten, feilsøke problemer med programproxykoblingen, for å finne ut om programproxykontakter er riktig konfigurert. Hvis du fremdeles har problemer med å koble til programmet, kan du følge feilsøkingsflyten i problemer med [programproxyprogrammet Feilsøking.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Du kan [identifisere CORS-problemer](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) ved hjelp av feilsøkingsverktøy for nettleseren:
    - Start nettleseren, og bla til nettappen.
    - Trykk **F12** for å hente frem feilsøkingskonsollen.
    - Prøv å reprodusere transaksjonen, og se gjennom konsollmeldingen. Et KORS-brudd gir en konsollfeil om opprinnelsen.
    - Noen CORS-problemer kan ikke løses, for eksempel når appen omdirigerer til login.microsoft.com godkjenning, og tilgangstokenet utløper. CORS-anropet mislykkes deretter. En midlertidig løsning for dette scenariet er å utvide levetiden for tilgangstokenet for å hindre at den utløper under en brukers økt. Hvis du vil ha mer informasjon om hvordan du gjør dette, kan du se [Konfigurerbare levetider for token i Microsoft Identity-plattformen.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
4. **Feilsøking av SAML-basert** enkel pålogging: Vi anbefaler at du kontrollerer problemer med å logge på [SAML-baserte,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)konfigurerte apper for enkel pålogging, for å finne løsningen på problemene du mest sannsynlig vil støte på.
5. **Feilsøking av passordbasert** enkel pålogging: Vi anbefaler å kontrollere Feilsøke passordbasert enkel pålogging i [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)for å finne løsningene på problemene du mest sannsynlig vil støte på.
6. Hvis du har tilkoblingsproblemer når du bruker et VPN, kan du se Hvordan bruke enkel pålogging [(SSO) over VPN og](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)Wi-Fi tilkoblinger.
