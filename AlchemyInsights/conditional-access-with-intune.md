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
# <a name="conditional-access-with-intune"></a><span data-ttu-id="bd47b-102">Betinget tilgang med Intune</span><span class="sxs-lookup"><span data-stu-id="bd47b-102">Conditional Access with Intune</span></span>

<span data-ttu-id="bd47b-103">Bruk  **av betinget**  tilgang med Intune krever tre trinn:</span><span class="sxs-lookup"><span data-stu-id="bd47b-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="bd47b-104">Opprett en  **samsvarspolicy**  ([Android,](https://docs.microsoft.com/intune/compliance-policy-create-android)  [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios)  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) for å definere innstillinger som må være oppfylt før enheten overholdes.</span><span class="sxs-lookup"><span data-stu-id="bd47b-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="bd47b-105">En enhet må for eksempel ha en PIN-kode med minst seks sifre før den overholder samsvarsoverensstemmelsen.</span><span class="sxs-lookup"><span data-stu-id="bd47b-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="bd47b-106">Opprett en **policy for betinget**  tilgang som definerer hvilke ressurser som beskyttes, og hvilke betingelser som må være oppfylt for å få tilgang til disse ressursene.</span><span class="sxs-lookup"><span data-stu-id="bd47b-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="bd47b-107">[En enhet må for](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  eksempel samsvare før du kan få tilgang til bedriftens e-post.</span><span class="sxs-lookup"><span data-stu-id="bd47b-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="bd47b-108">Sikre at **både samsvarspolicyer**  og  **policyer for**  betinget tilgang er rettet mot de ønskede brukergruppene.</span><span class="sxs-lookup"><span data-stu-id="bd47b-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="bd47b-109">Dette kan kreve at du oppretter bestemte brukergrupper i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bd47b-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="bd47b-110">**Nyttige koblinger:**</span><span class="sxs-lookup"><span data-stu-id="bd47b-110">**Helpful links:**</span></span>

[<span data-ttu-id="bd47b-111">Oversikt over enhetssamsvar</span><span class="sxs-lookup"><span data-stu-id="bd47b-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="bd47b-112">Feilsøking av sertifiseringsinstans</span><span class="sxs-lookup"><span data-stu-id="bd47b-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="bd47b-113">Feilsøking av policy</span><span class="sxs-lookup"><span data-stu-id="bd47b-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="bd47b-114">To protect Email (Exchange Online) from access by noncompliant devices, both documents must be followed:</span><span class="sxs-lookup"><span data-stu-id="bd47b-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="bd47b-115">Beskytte e-posttilgang fra enheter ved hjelp av EAS</span><span class="sxs-lookup"><span data-stu-id="bd47b-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="bd47b-116">Beskytte e-posttilgang fra enheter ved hjelp av klienter for moderne godkjenning som Outlook</span><span class="sxs-lookup"><span data-stu-id="bd47b-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)