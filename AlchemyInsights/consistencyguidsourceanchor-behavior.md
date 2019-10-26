---
title: ConsistencyGuid/sourceAnchor-oppførsel
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
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/25/2019
ms.locfileid: "36517000"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor-oppførsel

Azure AD Connect (versjon 1.1.524.0 og etter) forenkler nå bruken av muskel-og skjelettlidelser-ConsistencyGuid som sourceAnchor-attributt. Når du bruker denne funksjonen, konfigurerer Azure AD-tilkobling automatisk synkroniserings reglene til:
  
- Bruk muskel-ConsistencyGuid som sourceAnchor-attributt for User-objekter. ObjectGUID brukes for andre objekttyper.
    
- For en gitt lokale AD brukerobjekt som muskel-ConsistencyGuid-attributtet ikke er fylt ut, skriver Azure AD Connect sin objectGUID-verdi tilbake til attributtet muskel-ConsistencyGuid i lokale Active Directory. Når ConsistencyGuid-attributtet er fylt ut, eksporterer Azure AD koble deretter objektet til Azure AD.
    
 **Merk:** Når en lokale AD-objektet er importert til Azure AD-tilkobling (det vil si importert til AD Connector-plass og projisert i metaverse), kan du ikke endre sin sourceAnchor-verdi lenger. Hvis du vil angi sourceAnchor-verdien for et gitt lokale AD-objekt, kan du konfigurere attributtet for muskel-ConsistencyGuid før det importeres til Azure AD-tilkobling. 
  
Hvis du vil ha mer informasjon om SourceAnchor og ConsistencyGuid, kan du se følgende: [Azure ad-tilkobling: design konsepter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

