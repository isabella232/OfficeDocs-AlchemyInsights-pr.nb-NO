---
title: KonsekvensGuid/ sourceAnchor-virkemåte
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817001"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>KonsekvensGuid/ sourceAnchor-virkemåte

Azure AD Connect (versjon 1.1.524.0 og etter) forenkler nå bruken av msDS-ConsistencyGuid som sourceAnchor-attributt. Når du bruker denne funksjonen, konfigurerer Azure AD Connect automatisk synkroniseringsreglene til å:
  
- Bruk msDS-ConsistencyGuid som sourceAnchor-attributt for brukerobjekter. ObjectGUID brukes for andre objekttyper.
    
- For et gitt lokalt AD User-objekt der msDS-ConsistencyGuid-attributtet ikke er fylt ut, skriver Azure AD Connect objektGUID-verdien tilbake til msDS-ConsistencyGuid-attributtet i lokal Active Directory. Når msDS-ConsistencyGuid-attributtet er fylt ut, eksporterer Azure AD Connect deretter objektet til Azure AD.
    
 **Obs!** Når et lokalt AD-objekt er importert til Azure AD Connect (det vil si importert til AD Connector Space og projiseres til Metaverse), kan du ikke endre sourceAnchor-verdien lenger. Hvis du vil angi sourceAnchor-verdien for et gitt lokalt AD-objekt, konfigurerer du attributtet msDS-ConsistencyGuid før det importeres til Azure AD Connect. 
  
Hvis du vil ha mer informasjon om SourceAnchor og Konsekvensguid, kan du se følgende: [Azure AD Connect: Utformingskonsepter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

