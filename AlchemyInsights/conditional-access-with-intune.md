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
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807668"
---
# <a name="conditional-access-with-intune"></a>Betinget tilgang med Intune

Bruk av  **betinget tilgang**  med Intune krever tre trinn:

- Opprett en  **Overholdelses policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [IOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) for å definere innstillinger som må oppfylles før enheten anses å være kompatibel. En enhet må for eksempel ha en PIN-kode på minst 6 sifre før den anses som kompatibel.
- Opprett en **policy for betinget tilgang**  som definerer hvilke ressurser som skal beskyttes, og hvilke betingelser som må oppfylles for å få tilgang til disse ressursene.  En enhet må [for eksempel](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) være kompatibel før du kan få tilgang til e-postfirma.
- Kontroller at både **samsvars policyer**  og  **policyer for betinget tilgang**  er rettet mot de ønskede gruppene av brukere. Dette kan kreve at du oppretter bestemte grupper av brukere i Azure Active Directory.

**Nyttige koblinger:**

[Oversikt over enhets samsvar](https://docs.microsoft.com/intune/device-compliance-get-started)

[Feilsøke sertifiserings instans](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Feil søkings policy](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Hvis du vil beskytte e-post (Exchange Online) fra Access via ikke-kompatible enheter, må begge dokumentene følges:

1. [Beskytte e-posttilgang fra enheter ved hjelp av EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Beskytte e-posttilgang fra enheter ved hjelp av moderne godkjennings klienter som Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)