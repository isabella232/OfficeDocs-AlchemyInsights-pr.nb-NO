---
title: ConsistencyGuid/sourceAnchor-virkemåte
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756292"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor-virkemåte

Azure AD Connect (versjon 1.1.524.0 og etter) forenkler nå bruken av msDS-ConsistencyGuid som sourceAnchor-attributt. Når du bruker denne funksjonen, konfigurerer Azure AD Connect automatisk synkroniserings reglene til:
  
- Bruk msDS-ConsistencyGuid som sourceAnchor-attributt for bruker objekter. ObjectGUID brukes for andre objekt typer.
    
- For et hvilket som helst lokalt AD-brukerobjekt der attributtet msDS-ConsistencyGuid ikke er fylt ut, skriver Azure AD Connect sin objectGUID-verdi tilbake til msDS-ConsistencyGuid-attributtet i lokal Active Directory. Når attributtet msDS-ConsistencyGuid er fylt ut, eksporterer Azure AD Connect deretter objektet til Azure AD.
    
 **Obs!** Når et lokalt AD-objekt er importert til Azure AD Connect (som er importert til AD Connector-området og projisert til metaverse), kan du ikke endre sourceAnchor-verdien lenger. Hvis du vil angi sourceAnchor-verdien for et gitt lokalt AD-objekt, konfigurerer du attributtet msDS-ConsistencyGuid før det importeres til Azure AD Connect. 
  
Hvis du vil ha mer informasjon om SourceAnchor og ConsistencyGuid, kan du se følgende: [Azure ad Connect: utformings konsepter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

