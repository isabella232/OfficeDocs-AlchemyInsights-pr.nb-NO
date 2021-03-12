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
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704795"
---
# <a name="conditional-access-with-intune"></a>Betinget tilgang med Intune

Bruk  **av betinget**  tilgang med Intune krever tre trinn:

- Opprett en  **samsvarspolicy**  ([Android,](https://docs.microsoft.com/intune/compliance-policy-create-android)  [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios)  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) for å definere innstillinger som må være oppfylt før enheten overholdes. En enhet må for eksempel ha en PIN-kode med minst seks sifre før den overholder samsvarsoverensstemmelsen.
- Opprett en **policy for betinget**  tilgang som definerer hvilke ressurser som beskyttes, og hvilke betingelser som må være oppfylt for å få tilgang til disse ressursene.  [En enhet må for](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  eksempel samsvare før du kan få tilgang til bedriftens e-post.
- Sikre at **både samsvarspolicyer**  og  **policyer for**  betinget tilgang er rettet mot de ønskede brukergruppene. Dette kan kreve at du oppretter bestemte brukergrupper i Azure Active Directory.

**Nyttige koblinger:**

[Oversikt over enhetssamsvar](https://docs.microsoft.com/intune/device-compliance-get-started)

[Feilsøking av sertifiseringsinstans](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Feilsøking av policy](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

To protect Email (Exchange Online) from access by noncompliant devices, both documents must be followed:

1. [Beskytte e-posttilgang fra enheter ved hjelp av EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Beskytte e-posttilgang fra enheter ved hjelp av klienter for moderne godkjenning som Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)