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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044349"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>KonsekvensGuid/ sourceAnchor-virkemåte

Azure AD Koble til (versjon 1.1.524.0 og etter) forenkler nå bruken av msDS-ConsistencyGuid som sourceAnchor-attributt. Når du bruker denne funksjonen, konfigurerer Azure AD Koble til automatisk synkroniseringsreglene til:
  
- Bruk msDS-ConsistencyGuid som sourceAnchor-attributt for brukerobjekter. ObjectGUID brukes for andre objekttyper.
    
- For et gitt lokalt AD User-objekt som har msDS-ConsistencyGuid-attributtet ikke er fylt ut, skriver Azure AD Koble til sin objectGUID-verdi tilbake til msDS-ConsistencyGuid-attributtet i lokal Active Directory. Når attributtet msDS-ConsistencyGuid er fylt ut, eksporterer Azure AD Koble til deretter objektet til Azure AD.
    
 **Obs!** Når et lokalt AD-objekt er importert til Azure AD Koble til (det vil si importert til AD-koblingsområdet og projiseres til Metaverse), kan du ikke endre sourceAnchor-verdien lenger. Hvis du vil angi sourceAnchor-verdien for et gitt lokalt AD-objekt, konfigurerer du attributtet msDS-ConsistencyGuid før det importeres til Azure AD Koble til. 
  
Hvis du vil ha mer informasjon om SourceAnchor og Konsekvensguid, kan du se følgende: [Azure AD Koble til: Utformingskonsepter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

