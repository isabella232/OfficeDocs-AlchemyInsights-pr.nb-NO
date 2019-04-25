---
title: ConsistencyGuid / sourceAnchor virkemåte
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408117"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor virkemåte

Koble til Azure AD (versjon 1.1.524.0 og etter) nå forenkler bruken av msDS-ConsistencyGuid som sourceAnchor-attributtet. Når du bruker denne funksjonen, konfigurerer automatisk koble til Azure AD synkroniseringsregler til:
  
- Bruk msDS-ConsistencyGuid som sourceAnchor-attributt for brukerobjekter. ObjectGUID brukes for andre objekttyper.
    
- For en gitt lokale AD-bruker objektet der msDS-ConsistencyGuid-attributtet ikke er fylt ut på forhånd, Azure AD koble til skriver objectGUID verdien tilbake til msDS-ConsistencyGuid-attributtet i lokale Active Directory. Etter at attributtet msDS-ConsistencyGuid er fylt ut, eksporterer Azure AD-koble deretter objektet til Azure AD.
    
 **Merk:** En gang en lokale AD-objektet er importert til Azure AD-tilkobling (som er, importeres til AD Connector plass og forventet i Metaverse), kan du ikke endre verdien sourceAnchor lenger. Angi verdien for sourceAnchor for en gitt lokale AD objekt, konfigurere sin msDS-ConsistencyGuid-attributtet før den importeres til Azure AD-tilkobling. 
  
Hvis du vil ha mer informasjon om SourceAnchor og ConsistencyGuid, se følgende: [Azure AD-tilkobling: utforme konsepter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

