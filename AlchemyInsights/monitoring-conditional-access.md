---
title: Overvåke betinget tilgang
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28303695"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="3747d-102">Overvåke betinget tilgang</span><span class="sxs-lookup"><span data-stu-id="3747d-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="3747d-p101">Målrettet med betinget tilgang får brukere en e-postmelding med varsel hvis de ikke oppfyller tilgangskravene for din organisasjon. Hvis du vil løse, anbefales det at én eller flere av følgende løsninger:</span><span class="sxs-lookup"><span data-stu-id="3747d-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="3747d-p102">Hvis enheten er antas å være registrert, råder brukeren til å gå til Company Portal-app, og kontroller at vises det i Company Portal. Hvis ikke, bør du registrere enheten.</span><span class="sxs-lookup"><span data-stu-id="3747d-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="3747d-p103">Gå til i Azure portalen **Intune \> kompatibilitet for enheten**. Klikk **enheten kompatibilitet**under **skjermen** . Vis enhet-kompatibilitet rapporten til å bekrefte at brukerens enhet er merket som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="3747d-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="3747d-p104">Gå til i Azure portalen **Intune \> kompatibilitet for enheten**. Under **Administrer**Klikk **policyer**. Kontroller at det er tilordnet en profil til brukerens enhet i listen over samsvar policyer. Hvis ingen profil er tilordnet, vil deretter Intune ikke kunne bekrefte kompatibilitetsstatus for enheten.</span><span class="sxs-lookup"><span data-stu-id="3747d-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="3747d-114">Redigere tilordningen for brukerens betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="3747d-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="3747d-115">Gå til i Azure portalen **Intune \> betinget tilgang \> policyer for**</span><span class="sxs-lookup"><span data-stu-id="3747d-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="3747d-116">Velg en policy fra listen</span><span class="sxs-lookup"><span data-stu-id="3747d-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="3747d-117">Velg **brukere og grupper**</span><span class="sxs-lookup"><span data-stu-id="3747d-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="3747d-p105">Hvis du vil angi en bestemt policy på en person, kan du legge dem til **listen** . For å sikre at en person er utelatt fra policyen, kan du legge dem til i **Ekskluder** -listen.</span><span class="sxs-lookup"><span data-stu-id="3747d-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="3747d-120">Les mer: [Slik skjerm betinget tilgang enheter](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="3747d-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span></span>
  

