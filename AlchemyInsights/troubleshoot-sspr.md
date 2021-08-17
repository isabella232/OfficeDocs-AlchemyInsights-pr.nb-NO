---
title: Feilsøke SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038967"
---
# <a name="troubleshoot-sspr"></a>Feilsøke SSPR

**Jeg har problemer med å konfigurere tilbakestilling av passord**

- Hvis du er administrator og ser etter hvordan du aktiverer selvbetjent tilbakestilling av passord, kan du se Opplæring aktivere [SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)for å konfigurere tilbakestilling av passord for organisasjonen. Du kan også se gjennom [lisenskravene](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support). Du må ha minst én lisens tilordnet i organisasjonen.
    - **Skybrukere –** alle Office 365 (O365) betalt SKU eller Azure AD Basic
    - **Sky- og/eller lokale** brukere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
- Hvis du vil ha flere spørsmål om selvbetjent tilbakestilling av passord, kan du se [vanlige spørsmål.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jeg får en feilmelding**

Se gjennom denne artikkelen for å finne vanlige feil og løsningene deres: [Feilsøke selvbetjent tilbakestilling av passord](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jeg har et problem med policyen for tilbakestilling av passord**

- Hvis policyen for tilbakestilling av passord ikke oppfører seg som [forventet,](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)eller hvis du har spørsmål om policyer for tilbakestilling av passord, kan du se gjennom denne artikkelen: Passordpolicyer og begrensninger i Azure Active Directory .
- Policyer for tilbakestilling av passord gjelder ikke for administratorer. Microsoft håndhever en sterk standard policy for tilbakestilling av passord med to porter for enhver Azure-administratorrolle. Kontroller at du tester med en bruker som ikke er administrator. Hvis du vil ha mer informasjon om policyen for tilbakestilling av administrator, kan du se denne artikkelen: [Policyforskjeller for tilbakestilling av administrator](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**Jeg vil ikke at brukerne skal registrere mer sikkerhetsinformasjon for tilbakestilling av passord**

Du kan forhåndsutligne data (e-post- og telefonattributter) for brukerne ved hjelp av en API, PowerShell eller Azure AD-Koble til. Slik finner du ut hvordan du leser:

- [Distribuere tilbakestilling av passord uten at brukerne må registrere seg](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Hvilke data som brukes av tilbakestilling av passord](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jeg vil at brukerne skal registrere den ekstra sikkerhetsinformasjonen for tilbakestilling av passord**

1. Be brukerne registrere sikkerhetsinformasjonen for selvbetjent tilbakestilling av passord ved å be dem om å [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Når dataene er fylt ut for brukeren (av brukeren eller administratoren), kan du be brukeren om å aka.ms/sspr slik [at](https://passwordreset.microsoftonline.com/) brukerne kan få mulighet til å tilbakestille sine egne passord.
1. Hvis brukere fremdeles har problemer, er de mest **sannsynlige** brukere i forbund eller brukere med **hash for passordsynkronisert.** Dette betyr at det sannsynligvis er et problem med writeback-tjenesten for passord.