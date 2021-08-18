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
ms.openlocfilehash: c32ab88a72c265be411350e50756f5b2e1e3337c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322140"
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

**Obs!** Dette fungerer ikke for lisenskombinasjoner som: Win E5 + O365 E5 + EMS E5. Du må ha en ren M365 E5-lisens for å konfigurere denne funksjonen.

Hvis du vil ha mer informasjon om endepunkt-DLP-lisensiering, kan du [se Endepunkt-DLP-lisensiering.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
