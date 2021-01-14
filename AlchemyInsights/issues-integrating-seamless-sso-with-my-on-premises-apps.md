---
title: Problemer med integrering av sømløst SSO med de lokale appene
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
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868718"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemer med integrering av sømløst SSO med de lokale appene

Hvis du vil feilsøke problemer med integrering av sømløst SSO med lokale programmer, gjør du følgende:

**Anbefalte trinn**

1. Hvis du vil konfigurere et **lokalt program** for **enkel pålogging via program-proxy**, kan du se [passord hvelving for enkel pålogging med programproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Feilsøke proxy-problemer med programmet**: Vi anbefaler at du starter med å se gjennom feil søkings flyt, [Feilsøk program for proxy Connector-problemer](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), for å finne ut om proxy-koblinger for appen er konfigurert riktig. Hvis du fremdeles har problemer med å koble til programmet, følger du Fremgangs måten for feil søking i forbindelse med program for [proxy-program for Feilsøk](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Du kan [identifisere CORS-problemer](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) ved å bruke følgende feil søkings verktøy for nett:
    1. Start nett leseren, og gå til net tap pen.
    1. Trykk **F12** for å åpne Debug-konsollen.
    1. Prøv å gjenskape transaksjonen, og se gjennom konsoll meldingen. Et CORS-brudd gir en konsoll feil om opprinnelse.
    1. Noen CORS-problemer kan ikke løses, for eksempel når appen omdirigeres til login.microsoftonline.com for godkjenning, og tilgangstoken utløper. CORS-samtalen mislykkes. En midlertidig løsning for dette scenariet er å forlenge leve tiden til tilgangstoken for å hindre at det utløper under en brukers økt. Hvis du vil ha mer informasjon om hvordan du gjør dette, kan du se [konfigurerbare token-leve tid i Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Anbefalte dokumenter**

- [Konfigurere enkel pålogging til et program-proxy-program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML Single Sign-on for lokale programmer med programproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Forstå og løse problemer med proxy-CORS for Azure Active Directory-app](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Feilsøke konfigurasjoner med begrenset Kerberos-delegering for programproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)