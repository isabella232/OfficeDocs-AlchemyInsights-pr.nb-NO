---
title: Betinget tilgang med Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29482096"
---
# <a name="conditional-access-with-intune"></a>Betinget tilgang med Intune

Ved hjelp av **Betinget tilgang** med Intune krever 3 trinn: 
  
- Opprette en **Betinget tilgangspolicy** som definerer hvilke ressurser beskyttes og hva betingelser må være oppfylt for å få tilgang til disse ressursene. For eksempel, må en enhet være kompatibel før tilgang til firmaets e-post. 
    
- Opprette en **Policy for samsvar** for å definere innstillinger som må være oppfylt før enheten er vurdert som kompatible. En enhet må for eksempel ha en PIN-kode med minst 6 sifre før den regnes som kompatible. 
    
- Å sørge for **Både samsvar policyer** og **Policyer** for betinget tilgang er rettet mot de ønskede gruppene av brukere. Dette kan kreve å opprette bestemte grupper av brukere i Active Directory-Azure. 
    
Les mer
  
- [Rutiner for betinget tilgang](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [Komme i gang med betinget tilgang](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

