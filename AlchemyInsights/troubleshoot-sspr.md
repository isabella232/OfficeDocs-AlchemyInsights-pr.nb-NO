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
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430220"
---
# <a name="troubleshoot-sspr"></a>Feilsøke SSPR

**Jeg har problemer med å konfigurere tilbakestilling av passord**

- Hvis du er administrator og ser etter hvordan du aktiverer selvbetjent tilbakestilling av passord, kan du se Opplæring aktivere [SSPR og](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)konfigurere tilbakestilling av passord for organisasjonen. Du kan også se gjennom [lisensieringskravene.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Du må ha minst én lisens tilordnet i organisasjonen.
    - **Bare skybrukere** – alle Office 365 (O365) betalte SKU-er, eller Azure AD Basic
    - **Skybrukere og/eller** lokale brukere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
- Hvis du vil ha flere spørsmål om selvbetjent tilbakestilling av passord, kan du se [vanlige spørsmål.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jeg får en feilmelding**

Se gjennom denne artikkelen for å finne vanlige feil og løsninger for dem: [Feilsøke selvbetjent tilbakestilling av passord](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jeg har et problem med policyen for tilbakestilling av passord**

- Hvis policyen for tilbakestilling av passord ikke oppfører seg som forventet, eller hvis du har spørsmål om policyer for tilbakestilling av passord, kan du se denne artikkelen: Passordpolicyer og begrensninger i [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)
- Policyer for tilbakestilling av passord gjelder ikke for administratorer. Microsoft håndhever en sterk policy for tilbakestilling av passord med to porter for en hvilken som helst Azure-administratorrolle. Kontroller at du tester med en bruker som ikke er administrator. Hvis du vil ha mer informasjon om policyen for tilbakestilling av administrator, kan du se denne artikkelen: [Policyforskjeller for tilbakestilling av administratorer.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Jeg vil ikke at brukerne mine skal registrere mer sikkerhetsinformasjon for tilbakestilling av passord**

Du kan forhåndsutmulere data (e-post- og telefonattributter) for brukere som bruker en API, PowerShell eller Azure AD Connect. Slik finner du ut hvordan du leser:

- [Distribuere tilbakestilling av passord uten at brukere må registrere seg](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Hvilke data som brukes av tilbakestilling av passord](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jeg vil at brukerne skal registrere ekstra sikkerhetsinformasjon for tilbakestilling av passord**

1. Be brukerne registrere sin sikkerhetsinformasjon for selvbetjent tilbakestilling av passord ved å be dem [om](https://mysignins.microsoft.com/security-info)å aka.ms/ssprsetup.
1. Når dataene er fylt ut for brukeren (av brukeren eller av administratoren), dirigerer du brukeren til aka.ms/sspr slik [at](https://passwordreset.microsoftonline.com/) brukerne kan få mulighet til å tilbakestille sitt eget passord.
1. Hvis brukerne fremdeles har problemer, er de mest sannsynlige brukere **i** forbund eller brukere med **hash-hash for** passord. Dette betyr at det sannsynligvis er et problem med Password Writeback-tjenesten.