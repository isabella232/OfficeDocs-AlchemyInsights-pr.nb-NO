---
title: Trenger du å merke et domene eller en e-post avsender som sikker?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792141"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Trenger du å merke et domene eller en e-post avsender som sikker?

- Bruk av **lister over klarerte avsendere** anbefales ikke siden det åpner opp organisasjonen for søppelpost, phish og forfalskende angrep.
- Hvis det er et forretningskrav, anbefaler vi imidlertid **at** du bruker regler **[for](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** e-postflyt for dette. Veiledningen vår sikrer at avsendergodkjenning (bekrefter at sending av domene ikke forfalskes). **Obs!** Vi anbefaler ikke å behandle falske positiver ved å bruke lister over klarerte avsendere, fordi unntak fra søppelpostfiltrering kan åpne organisasjonen for sikkerhetsangrep. Hvis brukeren(e) mottar meldinger som er feil merket som søppelpost, kan du **[rapportere meldinger og filer til Microsoft](https://protection.office.com/reportsubmission)**.
- Klarerte avsendere i Outlook, listen over tillatte avsendere eller tillatte domener i søppelpostpolicyer bør unngås fordi avsendere omgår all søppelpost, forfalsket og phish-beskyttelse og avsendergodkjenning (SPF, DKIM, DMARC).  Denne metoden brukes best bare til midlertidig testing.
