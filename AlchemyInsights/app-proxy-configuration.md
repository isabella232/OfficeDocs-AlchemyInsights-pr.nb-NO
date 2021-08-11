---
title: Konfigurasjon av appproxy
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
- "9004356"
- "7800"
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951574"
---
# <a name="app-proxy-configuration"></a>Konfigurasjon av appproxy

1. Hvis du vil forstå hvordan du konfigurerer et Programproxy-program i Azure AD for å vise lokale programmer i skyen, kan du se Slik konfigurerer du [et program for programproxy](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. Enkel pålogging (SSO) gir brukerne tilgang til et program uten å godkjenne flere ganger. Den gjør at enkel godkjenning kan utføres i skyen, mot Azure Active Directory, og gjør at tjenesten eller koblingen kan representere brukeren for å fullføre eventuelle ekstra godkjenningsutfordringer fra programmet. Hvis du vil ha mer informasjon, kan du se Slik konfigurerer du enkel pålogging [til et programproxyprogram](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. Bruk [denne artikkelen til](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) å feilsøke vanlige problemer som personer står overfor når de oppretter et nytt program-proxy-program.
4. Hvis du har problemer med å konfigurere bakgodkjenning til programmet, må du kanskje feilsøke [Kerberos begrensede delegeringskonfigurasjoner for](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) Programproxy eller følge veiledningen for å konfigurere programmet med [PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) for å løse problemet.
