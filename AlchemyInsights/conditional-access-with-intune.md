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
# <a name="conditional-access-with-intune"></a><span data-ttu-id="85c23-102">Betinget tilgang med Intune</span><span class="sxs-lookup"><span data-stu-id="85c23-102">Conditional Access with Intune</span></span>

<span data-ttu-id="85c23-103">Bruk av **betinget tilgang** med Intune krever 3 trinn:</span><span class="sxs-lookup"><span data-stu-id="85c23-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="85c23-104">Opprett en **samsvarspolicy** ([Android,](https://docs.microsoft.com/intune/compliance-policy-create-android) [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) for å definere innstillinger som må oppfylles før enheten anses som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="85c23-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="85c23-105">En enhet må for eksempel ha en pin på minst 6 sifre før den anses som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="85c23-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="85c23-106">Opprett en **policy for betinget tilgang** som definerer hvilke ressurser som beskyttes, og hvilke betingelser som må oppfylles for å få tilgang til disse ressursene.</span><span class="sxs-lookup"><span data-stu-id="85c23-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="85c23-107">[En](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) enhet må for eksempel være kompatibel før du åpner bedriftens e-post.</span><span class="sxs-lookup"><span data-stu-id="85c23-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="85c23-108">Kontroller at både **samsvarspolicyer** og **policyer** for betinget tilgang er rettet mot de ønskede brukergruppene.</span><span class="sxs-lookup"><span data-stu-id="85c23-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="85c23-109">Dette kan kreve oppretting av bestemte grupper av brukere i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="85c23-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="85c23-110">**Nyttige lenker:**</span><span class="sxs-lookup"><span data-stu-id="85c23-110">**Helpful links:**</span></span>

[<span data-ttu-id="85c23-111">Oversikt over enhetssamsvar</span><span class="sxs-lookup"><span data-stu-id="85c23-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="85c23-112">Feilsøking av SERTIFISERINGSINSTANs</span><span class="sxs-lookup"><span data-stu-id="85c23-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="85c23-113">Feilsøking av retningslinjer</span><span class="sxs-lookup"><span data-stu-id="85c23-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="85c23-114">Hvis du vil beskytte e-post (Exchange online) fra tilgang fra ikke-samsvarende enheter, må begge dokumentene følges:</span><span class="sxs-lookup"><span data-stu-id="85c23-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="85c23-115">Beskytt e-posttilgang fra enheter ved hjelp av EAS</span><span class="sxs-lookup"><span data-stu-id="85c23-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="85c23-116">Beskytt e-posttilgang fra enheter ved hjelp av moderne godkjenningsklienter som Outlook</span><span class="sxs-lookup"><span data-stu-id="85c23-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)