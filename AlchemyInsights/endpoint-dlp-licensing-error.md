---
title: Lisensierings feil for Endpoint DLP
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
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564614"
---
# <a name="endpoint-dlp-licensing-error"></a>Lisensierings feil for Endpoint DLP

Når du prøver å konfigurere Endpoint DLP, får du følgende feil melding:

`Your organization is missing the licenses required to manage these devices`.

Kontroller at du har ett av følgende abonnementer eller tilleggs programmer:

- Microsoft 365 E5
- Microsoft 365 a5 (EDU)
- Microsoft 365 E5-kompatibilitet
- Samsvar med Microsoft 365 a5
- Microsoft 365 E5-informasjons beskyttelse og styring
- Microsoft 365 a5-informasjons beskyttelse og styring

> [!NOTE]
> Dette vil ikke fungere for lisens kombinasjoner som: Win E5 + O365 E5 + EMS E5. Du må ha en ren M365 E5-lisens for å konfigurere denne funksjonen.

Hvis du vil ha mer informasjon om DLP-lisensiering, kan du se [ENDPOINT DLP-lisensiering.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
