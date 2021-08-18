---
title: Feil i DLP-lisensiering for endepunkt
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: 1e242abe18717e5ef64d6f067ab3ec6fa8833cb672dd21c85e577ce640240ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090158"
---
# <a name="endpoint-dlp-licensing-error"></a>Feil i DLP-lisensiering for endepunkt

Hvis du får følgende feilmelding når du prøver å konfigurere endepunkt-DLP:

`Your organization is missing the licenses required to manage these devices`.

Kontroller at du har ett av følgende abonnementer eller tillegg:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 samsvar
- Microsoft 365 A5 samsvar
- Microsoft 365 E5 informasjonsbeskyttelse og styring
- Microsoft 365 A5 informasjonsbeskyttelse og styring

> [!NOTE]
> Dette fungerer ikke for lisenskombinasjoner som: Win E5 + O365 E5 + EMS E5. Du må ha en ren M365 E5-lisens for å konfigurere denne funksjonen.

Hvis du vil ha mer informasjon om endepunkt-DLP-lisensiering, kan du se [Endepunkt-DLP-lisensiering.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
