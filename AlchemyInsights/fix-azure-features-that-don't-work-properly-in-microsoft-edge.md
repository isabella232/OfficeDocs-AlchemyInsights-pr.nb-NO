---
title: Gjør dette hvis Azure-funksjoner ikke fungerer som de skal i Microsoft Edge
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
- "9004128"
- "7206"
ms.openlocfilehash: e188ecb375f3d84b45a1a7718b3c0b797c756f822ba64b3824976fe79c1e8298
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54117097"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Gjør dette hvis Azure-funksjoner ikke fungerer som de skal i Microsoft Edge

Microsoft Edge har [kjente problemer](https://go.microsoft.com/fwlink/?linkid=2140608) som er relatert til sikkerhetssoner og kan påvirke hvordan Azure-brukere logger på Windows administrasjonssenteret. Hvis du har problemer med å bruke Azure-funksjoner Microsoft Edge, kan du prøve følgende trinn:

1. Søk etter **Alternativer** for Internett på **Start-menyen,** og velg det.
2. Gå til **Sikkerhet-fanen** i dialogboksen Egenskaper **for** Internett.
3. Velg **sonen Klarerte** nettsteder, og velg deretter **Områder-knappen.**
4. Legg til **nettadressen** for gatewayen i dialogboksen Klarerte områder, [https://login.microsoftonline.com](https://login.microsoftonline.com) og velg deretter [https://login.live.com](https://login.live.com) **Lukk**.
5. Gå til **Personvern-fanen** i dialogboksen Egenskaper **for** Internett.
6. I **Popup-blokkering-delen** velger du **Innstillinger**. Legg til nettadressen for gatewayen i dialogboksen som åpnes, i tillegg [https://login.microsoftonline.com](https://login.microsoftonline.com) til og , og velg deretter [https://login.live.com](https://login.live.com) **Lukk**.
