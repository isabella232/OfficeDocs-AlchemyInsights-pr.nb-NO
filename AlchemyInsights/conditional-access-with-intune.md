---
title: Betinget tilgang med Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29935954"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="debcb-102">Betinget tilgang med Intune</span><span class="sxs-lookup"><span data-stu-id="debcb-102">Conditional Access with Intune</span></span>

<span data-ttu-id="debcb-103">Ved hjelp av **Betinget tilgang** med Intune krever 3 trinn:</span><span class="sxs-lookup"><span data-stu-id="debcb-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="debcb-p101">Opprette en **Betinget tilgangspolicy** som definerer hvilke ressurser beskyttes og hva betingelser må være oppfylt for å få tilgang til disse ressursene. For eksempel, må en enhet være kompatibel før tilgang til firmaets e-post.</span><span class="sxs-lookup"><span data-stu-id="debcb-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="debcb-p102">Opprette en **Policy for samsvar** for å definere innstillinger som må være oppfylt før enheten er vurdert som kompatible. En enhet må for eksempel ha en PIN-kode med minst 6 sifre før den regnes som kompatible.</span><span class="sxs-lookup"><span data-stu-id="debcb-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="debcb-p103">Å sørge for **Både samsvar policyer** og **Policyer** for betinget tilgang er rettet mot de ønskede gruppene av brukere. Dette kan kreve å opprette bestemte grupper av brukere i Active Directory-Azure.</span><span class="sxs-lookup"><span data-stu-id="debcb-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="debcb-110">Les mer:</span><span class="sxs-lookup"><span data-stu-id="debcb-110">Read more:</span></span>
  
- [<span data-ttu-id="debcb-111">Rutiner for betinget tilgang</span><span class="sxs-lookup"><span data-stu-id="debcb-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="debcb-112">Komme i gang med betinget tilgang</span><span class="sxs-lookup"><span data-stu-id="debcb-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

