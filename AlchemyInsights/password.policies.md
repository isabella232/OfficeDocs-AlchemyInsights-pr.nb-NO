---
title: Passordpolicyer
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 12751288d04a2ec5993bf4a546b7d0c862f8f171f5bfd7a337cb79cb95792056
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040839"
---
# <a name="password-policies"></a>Passordpolicyer

**Jeg har problemer med passordpolicyen for en bruker**

- Passordpolicyen for en bruker avhenger av om brukeren bare er skybasert eller lokalt.
- Bare skybrukere må velge et passord som oppfyller kravene i denne artikkelen: Passordpolicyer som [bare gjelder for brukerkontoer i skyen](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- Lokale brukere må velge et passord som oppfyller de lokale kravene. Hvis en lokal bruker ikke kan angi passordet sitt, må du kontrollere lokale krav.

**Jeg vet ikke hvordan jeg angir eller kontrollerer utløpspolicyer for passord**

- Du kan angi og kontrollere utløpspolicyen for skybrukere i leieren ved hjelp av PowerShell. Følg instruksjonene i denne artikkelen: [Angi eller kontrollere passordpolicyene ved hjelp av PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- Policyen for passordutløp for lokale brukere er angitt i den lokale AD-en.

**Andre nyttige koblinger:**
- [Komme i gang med tilbakestilling av passord](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [Feilsøke administratorstartet tilbakestilling av passord](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
