---
title: Trenger du å merke et domene eller en e-post avsender trygt?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281180"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Trenger du å merke et domene eller en e-post avsender trygt?

- Bruk av **sikre avsenderlister anbefales ikke** siden den åpner opp organisasjonen for spam-, phish- og spoofing-angrep.
- Hvis det imidlertid er et forretningskrav, anbefaler vi **at** du bruker regler for **[e-postflyt](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for dette. Vår veiledning sikrer avsenderautentisering (bekrefter at sending av domene ikke blir forfalsket). **Merk:** Vi anbefaler ikke å administrere falske positiver ved hjelp av sikre avsenderlister, fordi unntak fra spamfiltrering kan åpne organisasjonen for sikkerhetsangrep. Hvis brukeren(e) mottar meldinger som er feilaktig merket som søppelpost eller søppelpost, må du **[rapportere meldinger og filer til Microsoft](https://protection.office.com/reportsubmission)**.
- Klarerte avsendere i Outlook, Tillatt avsenderliste eller tillatt domeneliste i policyer for anti-spam **bør unngås** fordi avsendere omgår all spam- og forfalskningsbeskyttelse og avsendergodkjenning (SPF, DKIM, DMARC). Denne metoden brukes best for midlertidig testing.
