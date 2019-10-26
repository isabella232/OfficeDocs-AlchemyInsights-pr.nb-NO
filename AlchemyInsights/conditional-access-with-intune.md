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
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/25/2019
ms.locfileid: "36505003"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="7e3bf-102">Betinget tilgang med Intune</span><span class="sxs-lookup"><span data-stu-id="7e3bf-102">Conditional Access with Intune</span></span>

<span data-ttu-id="7e3bf-103">Bruk av **betinget tilgang** med Intune krever tre trinn:</span><span class="sxs-lookup"><span data-stu-id="7e3bf-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="7e3bf-104">Opprett en **betinget tilgangs policy** som definerer hvilke ressurser som beskyttes, og hvilke betingelser som må oppfylles for å få tilgang til disse ressursene.</span><span class="sxs-lookup"><span data-stu-id="7e3bf-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="7e3bf-105">En enhet må for eksempel være kompatibel før de får tilgang til firmaets e-post.</span><span class="sxs-lookup"><span data-stu-id="7e3bf-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="7e3bf-106">Opprette en **Samsvars policy** for å definere innstillinger som må oppfylles før enheten anses som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="7e3bf-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="7e3bf-107">En enhet må for eksempel ha en PIN-kode på minst 6 sifre før den anses som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="7e3bf-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="7e3bf-108">Å sikre både **samsvarspolicyer** og **policyer for betinget tilgang** er rettet mot de ønskede brukergruppene.</span><span class="sxs-lookup"><span data-stu-id="7e3bf-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="7e3bf-109">Dette kan kreve oppretting av bestemte brukergrupper i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7e3bf-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="7e3bf-110">Les mer:</span><span class="sxs-lookup"><span data-stu-id="7e3bf-110">Read more:</span></span>
  
- [<span data-ttu-id="7e3bf-111">Gode fremgangsmåter for betinget tilgang</span><span class="sxs-lookup"><span data-stu-id="7e3bf-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="7e3bf-112">Komme i gang med betinget tilgang</span><span class="sxs-lookup"><span data-stu-id="7e3bf-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

