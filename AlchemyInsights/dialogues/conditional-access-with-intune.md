---
title: Bruke betinget tilgang med Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694708"
---
# <a name="using-conditional-access-with-intune"></a>Bruke betinget tilgang med Intune

Bruk av betinget tilgang med Intune krever tre trinn:

- [Opprett en samsvarspolicy for å definere innstillinger som må være oppfylt før enheten regnes som kompatibel. En enhet må for eksempel ha en PIN-kode med minst seks sifre før den overholder samsvarsoverensstemmelsen.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Opprett en policy for betinget tilgang som definerer hvilke ressurser som beskyttes, og hvilke betingelser som må være oppfylt for å få tilgang til disse ressursene. En enhet må for eksempel samsvare før du kan få tilgang til bedriftens e-post.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Sikre at både samsvarspolicyer og policyer for betinget tilgang er rettet mot de ønskede brukergruppene. Dette kan kreve at du oppretter bestemte brukergrupper i Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Finn ut mer ...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
