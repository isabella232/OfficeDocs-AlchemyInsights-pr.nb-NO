---
title: Feilsøke problemer med Office 365 Advanced Threat Protection (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511121"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Feilsøke problemer med Office 365 ATP

- **Varselforsinkelser med levering av e-postmelding?** Prøv å bruke alternativet Dynamisk levering for policyene for ATP-sikre vedlegg. Dette vil unngå leveringsforsinkelser for e-postmeldinger samtidig som mottakerne beskyttes mot skadelige filer.
- **Vil du rapportere falske positive eller falske negativer?** Bruk denne koblingen til å sende inn filen din for analyse:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **Visste du at du kan aktivere ATP Safe Links beskyttelse for e-post sendt mellom personer i organisasjonen?** Følg disse trinnene:
    1. Gå til https://protection.office.com , og logg på.
    2. Gå **Threat management**til  >  **Sikker**  >  **koblinger**for trusselbehandling .
    3. Under **Policyer som gjelder for bestemte mottakere**, rediger (eller legg til) en policy.
    4. Velg **Bruk sikre koblinger på meldinger som sendes i organisasjonen**.
    5. Lagre retningslinjene dine, og la det gå omtrent 30 minutter før endringene fungerer seg gjennom datasenteret.
- Hvis du vil ha mer hjelp med ATP, kan du se [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).