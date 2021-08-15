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
ms.openlocfilehash: 7058b6419e52fce94f3359d0bd8e1d67c5aa5ef6743abf4ed39f45bad49e1d07
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025619"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Trenger du å merke et domene eller en e-post avsender som sikker?

- Bruk av **lister over klarerte avsendere** anbefales ikke siden det åpner opp organisasjonen for søppelpost, phish og forfalskende angrep.
- Hvis det er et forretningskrav, anbefaler vi imidlertid **at** du bruker **[E-Flow regler](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for dette. Veiledningen vår sikrer at avsendergodkjenning (bekrefter at sending av domene ikke forfalskes). **Obs!** Vi anbefaler ikke å behandle falske positiver ved å bruke lister over klarerte avsendere, fordi unntak fra søppelpostfiltrering kan åpne organisasjonen for sikkerhetsangrep. Hvis brukeren(e) mottar meldinger som er feil merket som søppelpost, kan du **[rapportere meldinger og filer til Microsoft](https://protection.office.com/reportsubmission)**.
- Safe Avsendere i Outlook, listen over tillatte avsendere eller  tillatte domener i søppelpostpolicyer bør unngås fordi avsendere omgår all søppelpost, forfalsket og phish-beskyttelse og avsendergodkjenning (SPF, DKIM, DMARC). Denne metoden brukes best bare til midlertidig testing.
- Valideringen som en bestemt **[e-post](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)** forbigikk Antispam-evalueringen, kan gjøres ved å kontrollere meldingshodet «X-Forefront-Antispam-Report» (SFV:SFE, SFV:SKA, SFV:SKN), se Meldingshoder for søppelpost .
- Fordi Microsoft ønsker å sikre kundene våre som [standard,](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)brukes ikke noen overstyringer av tenanter for skadelig programvare og phishing med høy sikkerhet. Disse overstyringene omfatter: o Tillatte avsenderlister eller tillatte domenelister (søppelpostpolicyer) o Outlook Safe Avsendere o tillatelsesliste for IP (tilkoblingsfiltrering) 
- Den eneste overstyringen som gjør at phishing-meldinger med høy sikkerhet kan hoppe over filtrering, er Exchange regler for e-postflyt (også kalt transportregler). Hvis du vil bruke regler for e-postflyt til å hoppe over filtrering, kan du se Bruke regler for e-postflyt til å angi søppelpostsikkerhetsnivået **[(SCL) i meldinger.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**