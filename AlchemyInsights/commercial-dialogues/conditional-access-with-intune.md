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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749257"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="bbc92-102">Bruke betinget tilgang med Intune</span><span class="sxs-lookup"><span data-stu-id="bbc92-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="bbc92-103">Bruk av betinget tilgang med Intune krever tre trinn:</span><span class="sxs-lookup"><span data-stu-id="bbc92-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="bbc92-104">Opprett en samsvarspolicy for å definere innstillinger som må oppfylles før enheten anses som kompatibel. En enhet må for eksempel ha en pin-kode på minst seks sifre før den anses som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="bbc92-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="bbc92-105">Opprett en policy for betinget tilgang som definerer hvilke ressurser som beskyttes, og hvilke betingelser som må oppfylles for å få tilgang til disse ressursene. En enhet må for eksempel være kompatibel før du får tilgang til bedriftens e-post.</span><span class="sxs-lookup"><span data-stu-id="bbc92-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="bbc92-106">Kontroller at både samsvarspolicyer og policyer for betinget tilgang er rettet mot de ønskede brukergruppene. Dette kan kreve at du oppretter bestemte grupper med brukere i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bbc92-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="bbc92-107">Finn ut mer ...</span><span class="sxs-lookup"><span data-stu-id="bbc92-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
