---
title: Trenger du å merke et domene eller en e-postavsender sikkert?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803254"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Trenger du å merke et domene eller en e-postavsender sikkert?

- Bruk av **klarerte avsender lister anbefales ikke** siden den åpner organisasjonen til søppel post, phish-og forfalsknings angrep.
- Hvis det imidlertid finnes et bedrifts krav, **anbefaler vi at** du bruker **[regler for e-postflyt](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for dette. Veiledningen vår sikrer at avsender godkjenning (bekrefter at du ikke forfalsker sending av domenet). **Obs**! vi anbefaler ikke administrering av falske positiver ved hjelp av lister over klarerte avsendere, fordi unntak til søppel post filtrering kan åpne organisasjonen din for å sikre sikkerhets angrep. Hvis brukeren (e) mottar meldinger som er feilaktig merket som søppel post eller søppel post, kan **[du rapportere meldinger og filer til Microsoft](https://protection.office.com/reportsubmission)**.
- Klarerte avsendere i Outlook, listen over tillatte avsender, eller listen over tillatte søppel post, **må unngås** fordi avsendere hopper over all søppel post, forfalsking og phish beskyttelse og avsender godkjenning (SPF, DKIM, DMARC). Denne metoden brukes best bare for midlertidig testing.
