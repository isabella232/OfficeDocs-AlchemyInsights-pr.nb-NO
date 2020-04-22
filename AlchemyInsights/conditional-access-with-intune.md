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
# <a name="conditional-access-with-intune"></a>Betinget tilgang med Intune

Bruk **av betinget tilgang** med Intune krever 3 trinn: 
  
- Opprett en **policy for betinget tilgang** som definerer hvilke ressurser som beskyttes, og hvilke betingelser som må oppfylles for å få tilgang til disse ressursene. En enhet må for eksempel være kompatibel før du åpner bedriftens e-post. 
    
- Opprett en **samsvarspolicy** for å definere innstillinger som må oppfylles før enheten anses som kompatibel. En enhet må for eksempel ha en pin på minst 6 sifre før den anses som kompatibel. 
    
- Sikre at både **samsvarspolicyer** og **policyer for betinget tilgang** er rettet mot de ønskede brukergruppene. Dette kan kreve oppretting av bestemte grupper av brukere i Azure Active Directory. 
    
Les mer:
  
- [Anbefalte fremgangsmåter for betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Komme i gang med betinget tilgang](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

