---
title: Problem med enkel pålogging for enkel pålogging
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
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935176"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Problem med enkel pålogging for enkel pålogging

Når brukeren er godkjent, bufrer nettleseren brukerens legitimasjon, slik at i samme nettleser logger programmet automatisk på med samme konto. Dette kan gjøre det vanskelig for en annen bruker eller en enkeltbruker å logge på flere kontoer på én enhet. Slik løser du dette: 1. Prøv å logge på en annen nettleser. 2. Tøm nettleserens buffer og/eller informasjonskapsler, og prøv å logge på på nytt.

Hvis du fremdeles har påloggingsproblemer, anbefaler vi følgende for å diagnostisere og automatisere løsningstrinnene:

1. Installer [utvidelsen mine apper for](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) sikker nettleser for å hjelpe Azure Active Directory (Azure AD) med å gi bedre diagnostisering og løsninger når du bruker testingen i Azure Portal.
2. Reproduser feilen ved hjelp av testopplevelsen på appkonfigurasjonssiden i Azure Portal. Hvis du vil ha mer informasjon, kan du se Feilsøke [SAML-baserte programmer for enkel pålogging.](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)
3. Hvis du bruker testopplevelsen i Azure-portalen med utvidelsen Mine apper sikker nettleser, kan du **hoppe over trinn 4.**
4. Slik åpner du den SAML-baserte konfigurasjonssiden for enkel pålogging:
    - Åpne [Azure-portalen,](https://portal.azure.com/) og logg på som **en global administrator** eller en **koadmin.**
    - Åpne **Azure Active Directory-utvidelsen** ved å velge **Alle tjenester** øverst i navigasjonsmenyen til venstre.
    - Skriv inn Azure Active Directory i filtersøkeboksen, og velg **Azure Active Directory-elementet.**
    - Velg **Enterprise-programmer** fra den venstre navigasjonsmenyen i Azure Active Directory.
    - Velg **Alle programmer** for å vise en liste over alle programmene. Hvis du ikke ser programmet du vil ha, vises her,  kan du bruke  **filterkontrollen** øverst i listen over alle programmer og angi Vis-alternativet til **Alle programmer.**
    - Velg programmet du vil konfigurere for enkel pålogging.
    - Når programmet lastes inn, velger du **Enkel** pålogging fra programmets venstre navigasjonsmeny.
    - Velg **SAML-basert SSO.**
5. Hvis du vil vite mer om de anbefalte trinnene du må følge, kan du se Problemer med å logge på [SAML-baserte,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)konfigurerte apper for enkel pålogging, basert på feilen.
6. Hvis du vil feilsøke andre brukerfeil, kan du se følgende veiledning:
    - [SAML-protokoll Sign-On enkel linje](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Slik feilsøker du påloggingsfeil ved hjelp av Azure Active Directory-rapporter](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Uventet spørsmål om samtykke](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Brukersamtykkefeil](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Problemer med å logge på fra Mine apper](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Feil på påloggingssiden for programmet](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Problem med å logge på en Microsoft-app](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
