---
title: Feilsøke problemer med passordbasert enkel pålogging (SSO)
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
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714881"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Feilsøke problemer med passordbasert enkel pålogging (SSO)

Hvis du vil lære det grunnleggende om passordbasert SSO, kan du se [passordbasert godkjenning med Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Konfigurere passordbasert SSO**

1. [Konfigurere passordbasert enkel pålogging](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – Denne artikkelen handler mer om det passordbaserte SSO-alternativet. Hvis programmet du legger til, krever egendefinert konfigurasjon og du må bruke passordbasert SSO, er denne artikkelen for deg.
2. [Konfigurere passordbasert enkel pålogging for](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) apper som er forhåndsinstallert – Programproxy støtter flere modus for enkel pålogging. Passordbasert pålogging er beregnet for programmer som bruker en brukernavn-/passordkombinasjon for godkjenning. Når du konfigurerer passordbasert pålogging for programmet, må brukerne logge seg på det lokale programmet én gang. Deretter lagrer Azure Active Directory påloggingsinformasjonen og automatisk gir den til programmet når brukerne får ekstern tilgang til det.
    - Du skal allerede ha publisert og testet appen med programproxy. Hvis ikke, følger du fremgangsmåten i Publiser programmer ved hjelp av Azure AD-programproxy, og deretter fortsetter du konfigurasjonen av passordbasert SSO for programmer som er forhåndsinstallert. [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application)

Hvis du vil feilsøke passordbasert SSO, kan du se [Feilsøke passordbasert](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) enkel pålogging i Azure AD
