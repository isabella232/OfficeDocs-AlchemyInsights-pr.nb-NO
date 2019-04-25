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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393550"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="9100e-102">Betinget tilgang med Intune</span><span class="sxs-lookup"><span data-stu-id="9100e-102">Conditional Access with Intune</span></span>

<span data-ttu-id="9100e-103">Ved hjelp av **Betinget tilgang** med Intune krever 3 trinn:</span><span class="sxs-lookup"><span data-stu-id="9100e-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="9100e-104">Opprette en **Betinget tilgangspolicy** som definerer hvilke ressurser beskyttes og hva betingelser må være oppfylt for å få tilgang til disse ressursene.</span><span class="sxs-lookup"><span data-stu-id="9100e-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="9100e-105">For eksempel, må en enhet være kompatibel før tilgang til firmaets e-post.</span><span class="sxs-lookup"><span data-stu-id="9100e-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="9100e-106">Opprette en **Policy for samsvar** for å definere innstillinger som må være oppfylt før enheten er vurdert som kompatible.</span><span class="sxs-lookup"><span data-stu-id="9100e-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="9100e-107">En enhet må for eksempel ha en PIN-kode med minst 6 sifre før den regnes som kompatible.</span><span class="sxs-lookup"><span data-stu-id="9100e-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="9100e-108">Å sørge for **Både samsvar policyer** og **Policyer** for betinget tilgang er rettet mot de ønskede gruppene av brukere.</span><span class="sxs-lookup"><span data-stu-id="9100e-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="9100e-109">Dette kan kreve å opprette bestemte grupper av brukere i Active Directory-Azure.</span><span class="sxs-lookup"><span data-stu-id="9100e-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="9100e-110">Les mer:</span><span class="sxs-lookup"><span data-stu-id="9100e-110">Read more:</span></span>
  
- [<span data-ttu-id="9100e-111">Rutiner for betinget tilgang</span><span class="sxs-lookup"><span data-stu-id="9100e-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="9100e-112">Komme i gang med betinget tilgang</span><span class="sxs-lookup"><span data-stu-id="9100e-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

