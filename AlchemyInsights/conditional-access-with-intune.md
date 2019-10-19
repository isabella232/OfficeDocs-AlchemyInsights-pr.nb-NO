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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36505003"
---
# <a name="conditional-access-with-intune"></a>Betinget tilgang med Intune

Bruk av **betinget tilgang** med Intune krever tre trinn: 
  
- Opprett en **betinget tilgangs policy** som definerer hvilke ressurser som beskyttes, og hvilke betingelser som må oppfylles for å få tilgang til disse ressursene. En enhet må for eksempel være kompatibel før de får tilgang til firmaets e-post. 
    
- Opprette en **Samsvars policy** for å definere innstillinger som må oppfylles før enheten anses som kompatibel. En enhet må for eksempel ha en PIN-kode på minst 6 sifre før den anses som kompatibel. 
    
- Å sikre både **samsvarspolicyer** og **policyer for betinget tilgang** er rettet mot de ønskede brukergruppene. Dette kan kreve oppretting av bestemte brukergrupper i Azure Active Directory. 
    
Les mer:
  
- [Gode fremgangsmåter for betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Komme i gang med betinget tilgang](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

