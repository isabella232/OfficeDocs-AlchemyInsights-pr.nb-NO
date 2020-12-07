---
title: Gjør dette hvis Azure-funksjonene ikke fungerer som de skal i Microsoft Edge
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
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583788"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Gjør dette hvis Azure-funksjonene ikke fungerer som de skal i Microsoft Edge

Microsoft Edge har [kjente problemer](https://go.microsoft.com/fwlink/?linkid=2140608) som er relatert til sikkerhets soner, og kan påvirke hvordan Azure-brukere logger seg på administrasjons senteret for Windows. Hvis du har problemer med å bruke Azure-funksjoner med Microsoft Edge, kan du prøve følgende trinn:

1. Søk etter **Alternativer for Internet t** på **Start** -menyen, og velg den.
2. Gå til fanen **sikkerhet** i dialog boksen **Egenskaper for Internet t** .
3. Velg sonen **Klarerte områder** , og velg deretter **områder** -knappen.
4. Legg til Netta DRESSen for gateway i tillegg til og i dialog boksen **Klarerte områder** , [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) og velg deretter **Lukk**.
5. Gå til **personvern** -fanen i dialog boksen **Egenskaper for Internet t** .
6. Velg **Innstillinger** i delen **popup-blokkering** . Legg til Netta DRESSen for gateway i tillegg til og i dialog boksen som åpnes, [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) og velg deretter **Lukk**.
