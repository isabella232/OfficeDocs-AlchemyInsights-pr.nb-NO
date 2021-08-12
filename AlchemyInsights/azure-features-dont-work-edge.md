---
title: Gjør dette hvis Azure-funksjoner ikke fungerer som de skal i Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: 710489bd7dcb10f5c953c83e87bdad030c47cfda7dbd38e1eceae78bfe0d8790
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812873"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Gjør dette hvis Azure-funksjoner ikke fungerer som de skal i Microsoft Edge

Microsoft Edge har kjente problemer relatert til sikkerhetssoner som kan påvirke hvordan Azure-brukere logger på Windows administrasjonssenteret. Hvis du vil ha mer informasjon, [kan du se Kjente problemer på Edge](https://go.microsoft.com/fwlink/?linkid=2140608). Hvis du har problemer med å bruke Azure-funksjoner med Microsoft Edge, kan du prøve følgende:

1. Skriv inn alternativer Start-meny Internett-alternativer i **søkefeltet** på **Start-meny,** og velg det.
1. Velg **Sikkerhet-fanen** **i** Egenskaper for Internett.
1. Velg **Klarerte nettsteder**, og velg deretter **Områder**.
1. Legg til nettadressen for gatewayen, i tillegg <https://login.microsoftonline.com> til og , og velg <https://login.live.com> **Lukk**.
1. Velg **Personvern-fanen** i Egenskaper **for** Internett.
1. I Popup-blokkering-delen velger du **Innstillinger**. Legg til nettadressen for gatewayen, i tillegg <https://login.microsoftonline.com> til og , og velg deretter <https://login.live.com> **Lukk**.