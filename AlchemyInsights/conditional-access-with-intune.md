---
title: Betinget tilgang med Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069721"
---
# <a name="conditional-access-with-intune"></a>Betinget tilgang med Intune

Bruk  **av betinget**  tilgang med Intune krever tre trinn:

- Opprett en **samsvarspolicy** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios) [, Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) for å definere innstillinger som må oppfylles før enheten anses som kompatibel. En enhet må for eksempel ha en pin-kode på minst seks sifre før den anses som kompatibel.
- Opprett en **policy for betinget**  tilgang som definerer hvilke ressurser som beskyttes, og hvilke betingelser som må oppfylles for å få tilgang til disse ressursene.  [En enhet må](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  for eksempel være kompatibel før du får tilgang til bedriftens e-post.
- Kontroller at **både samsvarspolicyer**  **og policyer for**  betinget tilgang er rettet mot de ønskede brukergruppene. Dette kan kreve at du oppretter bestemte grupper med brukere i Azure Active Directory.

**Nyttige koblinger:**

[Oversikt over enhetssamsvar](https://docs.microsoft.com/intune/device-compliance-get-started)

[Feilsøking av sertifiseringsinstans](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Feilsøkingspolicy](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Hvis du vil beskytte e-post (Exchange på nettet) mot tilgang fra ikke-kompatible enheter, må begge dokumentene følges:

1. [Beskytte e-posttilgang fra enheter ved hjelp av EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Beskytt e-posttilgang fra enheter ved hjelp av moderne godkjenningsklienter som Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)