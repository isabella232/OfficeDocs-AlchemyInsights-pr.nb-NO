---
title: Overvåke betinget tilgang
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29902364"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="0b6e2-102">Overvåke betinget tilgang</span><span class="sxs-lookup"><span data-stu-id="0b6e2-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="0b6e2-p101">Målrettet med betinget tilgang får brukere en e-postmelding med varsel hvis de ikke oppfyller tilgangskravene for din organisasjon. Hvis du vil løse, anbefales det at én eller flere av følgende løsninger:</span><span class="sxs-lookup"><span data-stu-id="0b6e2-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="0b6e2-p102">Hvis enheten er antas å være registrert, råder brukeren til å gå til Company Portal-app, og kontroller at vises det i Company Portal. Hvis ikke, bør du registrere enheten.</span><span class="sxs-lookup"><span data-stu-id="0b6e2-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="0b6e2-p103">Gå til i Azure portalen **Intune \> kompatibilitet for enheten**. Klikk **enheten kompatibilitet**under **skjermen** . Vis enhet-kompatibilitet rapporten til å bekrefte at brukerens enhet er merket som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="0b6e2-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="0b6e2-p104">Gå til i Azure portalen **Intune \> kompatibilitet for enheten**. Under **Administrer**Klikk **policyer**. Kontroller at det er tilordnet en profil til brukerens enhet i listen over samsvar policyer. Hvis ingen profil er tilordnet, vil deretter Intune ikke kunne bekrefte kompatibilitetsstatus for enheten.</span><span class="sxs-lookup"><span data-stu-id="0b6e2-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="0b6e2-114">Redigere tilordningen for brukerens betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="0b6e2-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="0b6e2-115">Gå til i Azure portalen **Intune \> betinget tilgang \> policyer for**</span><span class="sxs-lookup"><span data-stu-id="0b6e2-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="0b6e2-116">Velg en policy fra listen</span><span class="sxs-lookup"><span data-stu-id="0b6e2-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="0b6e2-117">Velg **brukere og grupper**</span><span class="sxs-lookup"><span data-stu-id="0b6e2-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="0b6e2-p105">Hvis du vil angi en bestemt policy på en person, kan du legge dem til **listen** . For å sikre at en person er utelatt fra policyen, kan du legge dem til i **Ekskluder** -listen.</span><span class="sxs-lookup"><span data-stu-id="0b6e2-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="0b6e2-120">Les mer: [Slik skjerm betinget tilgang enheter](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="0b6e2-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

