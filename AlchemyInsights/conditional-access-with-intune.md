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
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706030"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="ac54b-102">Betinget tilgang med Intune</span><span class="sxs-lookup"><span data-stu-id="ac54b-102">Conditional Access with Intune</span></span>

<span data-ttu-id="ac54b-103">Bruk **av betinget tilgang** med Intune krever 3 trinn:</span><span class="sxs-lookup"><span data-stu-id="ac54b-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="ac54b-104">Opprett en **policy for betinget tilgang** som definerer hvilke ressurser som beskyttes, og hvilke betingelser som må oppfylles for å få tilgang til disse ressursene.</span><span class="sxs-lookup"><span data-stu-id="ac54b-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="ac54b-105">En enhet må for eksempel være kompatibel før du åpner bedriftens e-post.</span><span class="sxs-lookup"><span data-stu-id="ac54b-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="ac54b-106">Opprett en **samsvarspolicy** for å definere innstillinger som må oppfylles før enheten anses som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="ac54b-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="ac54b-107">En enhet må for eksempel ha en pin på minst 6 sifre før den anses som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="ac54b-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="ac54b-108">Sikre at både **samsvarspolicyer** og **policyer for betinget tilgang** er rettet mot de ønskede brukergruppene.</span><span class="sxs-lookup"><span data-stu-id="ac54b-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="ac54b-109">Dette kan kreve oppretting av bestemte grupper av brukere i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ac54b-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="ac54b-110">Les mer:</span><span class="sxs-lookup"><span data-stu-id="ac54b-110">Read more:</span></span>
  
- [<span data-ttu-id="ac54b-111">Anbefalte fremgangsmåter for betinget tilgang</span><span class="sxs-lookup"><span data-stu-id="ac54b-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="ac54b-112">Komme i gang med betinget tilgang</span><span class="sxs-lookup"><span data-stu-id="ac54b-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

