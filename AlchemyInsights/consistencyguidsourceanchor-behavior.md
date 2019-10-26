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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="131f8-102">ConsistencyGuid/sourceAnchor-oppførsel</span><span class="sxs-lookup"><span data-stu-id="131f8-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="131f8-103">Azure AD Connect (versjon 1.1.524.0 og etter) forenkler nå bruken av muskel-og skjelettlidelser-ConsistencyGuid som sourceAnchor-attributt.</span><span class="sxs-lookup"><span data-stu-id="131f8-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="131f8-104">Når du bruker denne funksjonen, konfigurerer Azure AD-tilkobling automatisk synkroniserings reglene til:</span><span class="sxs-lookup"><span data-stu-id="131f8-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="131f8-105">Bruk muskel-ConsistencyGuid som sourceAnchor-attributt for User-objekter.</span><span class="sxs-lookup"><span data-stu-id="131f8-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="131f8-106">ObjectGUID brukes for andre objekttyper.</span><span class="sxs-lookup"><span data-stu-id="131f8-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="131f8-107">For en gitt lokale AD brukerobjekt som muskel-ConsistencyGuid-attributtet ikke er fylt ut, skriver Azure AD Connect sin objectGUID-verdi tilbake til attributtet muskel-ConsistencyGuid i lokale Active Directory.</span><span class="sxs-lookup"><span data-stu-id="131f8-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="131f8-108">Når ConsistencyGuid-attributtet er fylt ut, eksporterer Azure AD koble deretter objektet til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="131f8-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="131f8-109">**Merk:** Når en lokale AD-objektet er importert til Azure AD-tilkobling (det vil si importert til AD Connector-plass og projisert i metaverse), kan du ikke endre sin sourceAnchor-verdi lenger.</span><span class="sxs-lookup"><span data-stu-id="131f8-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="131f8-110">Hvis du vil angi sourceAnchor-verdien for et gitt lokale AD-objekt, kan du konfigurere attributtet for muskel-ConsistencyGuid før det importeres til Azure AD-tilkobling.</span><span class="sxs-lookup"><span data-stu-id="131f8-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="131f8-111">Hvis du vil ha mer informasjon om SourceAnchor og ConsistencyGuid, kan du se følgende: [Azure ad-tilkobling: design konsepter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="131f8-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

