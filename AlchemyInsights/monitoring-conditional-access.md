---
title: Overvåke betinget tilgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713727"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="a2e0e-102">Overvåke betinget tilgang for Exchange</span><span class="sxs-lookup"><span data-stu-id="a2e0e-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="a2e0e-103">Brukere som er målrettet med betinget tilgang, mottar en e-post om varsler hvis de ikke oppfyller organisasjonens tilgangskrav.</span><span class="sxs-lookup"><span data-stu-id="a2e0e-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="a2e0e-104">For å løse problemet anbefaler vi én eller flere av følgende løsninger:</span><span class="sxs-lookup"><span data-stu-id="a2e0e-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="a2e0e-105">Hvis enheten antas å være registrert, anbefaler du brukeren å gå til Firmaportal-appen og kontrollerer at den vises i firmaportalen.</span><span class="sxs-lookup"><span data-stu-id="a2e0e-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="a2e0e-106">Hvis den ikke gjør det, bør brukeren registrere enheten.</span><span class="sxs-lookup"><span data-stu-id="a2e0e-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="a2e0e-107">Gå til **Intune \> Device-samsvar i Azure-portalen.**</span><span class="sxs-lookup"><span data-stu-id="a2e0e-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="a2e0e-108">Klikk **Enhetssamsvar**under **Skjerm.**</span><span class="sxs-lookup"><span data-stu-id="a2e0e-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="a2e0e-109">Vis rapporten om enhetssamsvar for å kontrollere at brukerens enhet er merket som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="a2e0e-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="a2e0e-110">Gå til **Intune \> Device-samsvar i Azure-portalen.**</span><span class="sxs-lookup"><span data-stu-id="a2e0e-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="a2e0e-111">Klikk **Policyer**under **Behandle**.</span><span class="sxs-lookup"><span data-stu-id="a2e0e-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="a2e0e-112">Kontroller at en profil er tilordnet brukerens enhet i listen over samsvarspolicyer.</span><span class="sxs-lookup"><span data-stu-id="a2e0e-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="a2e0e-113">Hvis ingen profil er tilordnet, kan ikke Intune bekrefte enhetens samsvarsstatus.</span><span class="sxs-lookup"><span data-stu-id="a2e0e-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="a2e0e-114">Rediger brukerens betinget tilgangstilordning.</span><span class="sxs-lookup"><span data-stu-id="a2e0e-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="a2e0e-115">Gå til \*\*Intune Betingede tilgangspolicyer \> i Azure-portalen \> \*\*</span><span class="sxs-lookup"><span data-stu-id="a2e0e-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="a2e0e-116">Velg en policy fra listen</span><span class="sxs-lookup"><span data-stu-id="a2e0e-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="a2e0e-117">Klikk **brukere og grupper**</span><span class="sxs-lookup"><span data-stu-id="a2e0e-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="a2e0e-118">Hvis du vil målrette mot en bestemt policy hos noen, legger du dem til i **Inkluder-listen.**</span><span class="sxs-lookup"><span data-stu-id="a2e0e-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="a2e0e-119">Hvis du vil sikre at en person utelates fra policyen, legger du dem til i **Utelat-listen.**</span><span class="sxs-lookup"><span data-stu-id="a2e0e-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="a2e0e-120">Les mer: [Slik overvåker du enheter med betinget tilgang](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="a2e0e-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

