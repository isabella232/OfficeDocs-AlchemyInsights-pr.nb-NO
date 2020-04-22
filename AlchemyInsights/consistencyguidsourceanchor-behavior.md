---
title: ConsistencyGuid / sourceAnchor atferd
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705742"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor atferd

Azure AD Connect (versjon 1.1.524.0 og etter) forenkler nå bruken av msDS-ConsistencyGuid som sourceAnchor-attributt. Når du bruker denne funksjonen, konfigurerer Azure AD Connect automatisk synkroniseringsreglene til:
  
- Bruk msDS-ConsistencyGuid som sourceAnchor -attributtet for brukerobjekter. ObjectGUID brukes for andre objekttyper.
    
- For et gitt lokalt AD-brukerobjekt med msDS-ConsistencyGuid-attributtet ikke er fylt ut, skriver Azure AD Connect sin objectGUID-verdi tilbake til attributtet msDS-ConsistencyGuid i lokale Active Directory. Når attributtet msDS-ConsistencyGuid er fylt ut, eksporterer Azure AD Connect objektet til Azure AD.
    
 **Merk:** Når et lokalt AD-objekt er importert til Azure AD Connect (det vil si importert til AD Connector Space og projisert til Metaverse), kan du ikke endre sourceAnchor-verdien lenger. Hvis du vil angi sourceAnchor-verdien for et gitt lokalt AD-objekt, konfigurerer du attributtet msDS-ConsistencyGuid før det importeres til Azure AD Connect. 
  
Hvis du vil ha mer informasjon om SourceAnchor og ConsistencyGuid, kan du se følgende: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

