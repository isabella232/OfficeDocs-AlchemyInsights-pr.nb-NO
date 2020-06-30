---
title: Betinget tilgang med Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931445"
---
# <a name="conditional-access-with-intune"></a>Betinget tilgang med Intune

Bruk av **betinget tilgang** med Intune krever 3 trinn:

- Opprett en **samsvarspolicy** ([Android,](https://docs.microsoft.com/intune/compliance-policy-create-android) [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) for å definere innstillinger som må oppfylles før enheten anses som kompatibel. En enhet må for eksempel ha en pin på minst 6 sifre før den anses som kompatibel.
- Opprett en **policy for betinget tilgang** som definerer hvilke ressurser som beskyttes, og hvilke betingelser som må oppfylles for å få tilgang til disse ressursene.  [En](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) enhet må for eksempel være kompatibel før du åpner bedriftens e-post.
- Kontroller at både **samsvarspolicyer** og **policyer** for betinget tilgang er rettet mot de ønskede brukergruppene. Dette kan kreve oppretting av bestemte grupper av brukere i Azure Active Directory.

**Nyttige lenker:**

[Oversikt over enhetssamsvar](https://docs.microsoft.com/intune/device-compliance-get-started)

[Feilsøking av SERTIFISERINGSINSTANs](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Feilsøking av retningslinjer](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Hvis du vil beskytte e-post (Exchange online) fra tilgang fra ikke-samsvarende enheter, må begge dokumentene følges:

1. [Beskytt e-posttilgang fra enheter ved hjelp av EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Beskytt e-posttilgang fra enheter ved hjelp av moderne godkjenningsklienter som Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)