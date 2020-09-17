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
# <a name="conditional-access-with-intune"></a><span data-ttu-id="7075b-102">Betinget tilgang med Intune</span><span class="sxs-lookup"><span data-stu-id="7075b-102">Conditional Access with Intune</span></span>

<span data-ttu-id="7075b-103">Bruk av  **betinget tilgang**  med Intune krever tre trinn:</span><span class="sxs-lookup"><span data-stu-id="7075b-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="7075b-104">Opprett en  **Overholdelses policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [IOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) for å definere innstillinger som må oppfylles før enheten anses å være kompatibel.</span><span class="sxs-lookup"><span data-stu-id="7075b-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="7075b-105">En enhet må for eksempel ha en PIN-kode på minst 6 sifre før den anses som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="7075b-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="7075b-106">Opprett en **policy for betinget tilgang**  som definerer hvilke ressurser som skal beskyttes, og hvilke betingelser som må oppfylles for å få tilgang til disse ressursene.</span><span class="sxs-lookup"><span data-stu-id="7075b-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="7075b-107">En enhet må [for eksempel](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) være kompatibel før du kan få tilgang til e-postfirma.</span><span class="sxs-lookup"><span data-stu-id="7075b-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="7075b-108">Kontroller at både **samsvars policyer**  og  **policyer for betinget tilgang**  er rettet mot de ønskede gruppene av brukere.</span><span class="sxs-lookup"><span data-stu-id="7075b-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="7075b-109">Dette kan kreve at du oppretter bestemte grupper av brukere i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7075b-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="7075b-110">**Nyttige koblinger:**</span><span class="sxs-lookup"><span data-stu-id="7075b-110">**Helpful links:**</span></span>

[<span data-ttu-id="7075b-111">Oversikt over enhets samsvar</span><span class="sxs-lookup"><span data-stu-id="7075b-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="7075b-112">Feilsøke sertifiserings instans</span><span class="sxs-lookup"><span data-stu-id="7075b-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="7075b-113">Feil søkings policy</span><span class="sxs-lookup"><span data-stu-id="7075b-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="7075b-114">Hvis du vil beskytte e-post (Exchange Online) fra Access via ikke-kompatible enheter, må begge dokumentene følges:</span><span class="sxs-lookup"><span data-stu-id="7075b-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="7075b-115">Beskytte e-posttilgang fra enheter ved hjelp av EAS</span><span class="sxs-lookup"><span data-stu-id="7075b-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="7075b-116">Beskytte e-posttilgang fra enheter ved hjelp av moderne godkjennings klienter som Outlook</span><span class="sxs-lookup"><span data-stu-id="7075b-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)