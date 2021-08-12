---
title: Feilsøke problemer med passordbasert sømløs enkel pålogging (SSO)
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
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972833"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Feilsøke problemer med passordbasert sømløs enkel pålogging (SSO)

Hvis du vil lære det grunnleggende om passordbasert SSO, kan du se [Passordbasert godkjenning med Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Konfigurere passordbasert SSO**

1. [Konfigurere passordbasert enkel pålogging](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – Denne artikkelen inneholder mer detaljert informasjon om det passordbaserte SSO-alternativet. Hvis programmet du legger til, krever egendefinert konfigurasjon og du må bruke passordbasert SSO, er denne artikkelen for deg.
2. [Konfigurere passordbasert enkel pålogging for](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) apper som er forhåndsinstallert – Programproxy støtter flere moduser for enkel pålogging. Passordbasert pålogging er beregnet for programmer som bruker en kombinasjon av brukernavn/passord for godkjenning. Når du konfigurerer passordbasert pålogging for programmet, må brukerne logge på det lokale programmet én gang. Deretter lagrer Azure Active Directory påloggingsinformasjonen og gir den automatisk til programmet når brukerne får tilgang til den eksternt.
    - Du skal allerede ha publisert og testet appen med Programproxy. Hvis ikke, følger du fremgangsmåten i Publisere programmer ved hjelp av [Azure AD Application Proxy,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) og deretter fortsetter du konfigurasjonen av passordbasert SSO for forhåndsinstallert apper.

Hvis du vil feilsøke passordbasert SSO, kan du se [Feilsøke passordbasert enkel pålogging i Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
