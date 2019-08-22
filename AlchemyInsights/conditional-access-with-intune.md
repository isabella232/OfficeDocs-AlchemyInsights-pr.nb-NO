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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36505003"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="ea1be-102">Betinget tilgang med Intune</span><span class="sxs-lookup"><span data-stu-id="ea1be-102">Conditional Access with Intune</span></span>

<span data-ttu-id="ea1be-103">Ved hjelp av **Betinget tilgang** med Intune krever 3 trinn:</span><span class="sxs-lookup"><span data-stu-id="ea1be-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="ea1be-104">Opprette en **Betinget tilgangspolicy** som definerer hvilke ressurser beskyttes og hva betingelser må være oppfylt for å få tilgang til disse ressursene.</span><span class="sxs-lookup"><span data-stu-id="ea1be-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="ea1be-105">For eksempel, må en enhet være kompatibel før tilgang til firmaets e-post.</span><span class="sxs-lookup"><span data-stu-id="ea1be-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="ea1be-106">Opprette en **Policy for samsvar** for å definere innstillinger som må være oppfylt før enheten er vurdert som kompatible.</span><span class="sxs-lookup"><span data-stu-id="ea1be-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="ea1be-107">En enhet må for eksempel ha en PIN-kode med minst 6 sifre før den regnes som kompatible.</span><span class="sxs-lookup"><span data-stu-id="ea1be-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="ea1be-108">Å sørge for **Både samsvar policyer** og **Policyer** for betinget tilgang er rettet mot de ønskede gruppene av brukere.</span><span class="sxs-lookup"><span data-stu-id="ea1be-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="ea1be-109">Dette kan kreve å opprette bestemte grupper av brukere i Active Directory-Azure.</span><span class="sxs-lookup"><span data-stu-id="ea1be-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="ea1be-110">Les mer:</span><span class="sxs-lookup"><span data-stu-id="ea1be-110">Read more:</span></span>
  
- [<span data-ttu-id="ea1be-111">Rutiner for betinget tilgang</span><span class="sxs-lookup"><span data-stu-id="ea1be-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="ea1be-112">Komme i gang med betinget tilgang</span><span class="sxs-lookup"><span data-stu-id="ea1be-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

