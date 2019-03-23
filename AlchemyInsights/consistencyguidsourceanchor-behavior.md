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
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753111"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="6cf02-102">ConsistencyGuid / sourceAnchor virkemåte</span><span class="sxs-lookup"><span data-stu-id="6cf02-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="6cf02-103">Koble til Azure AD (versjon 1.1.524.0 og etter) nå forenkler bruken av msDS-ConsistencyGuid som sourceAnchor-attributtet.</span><span class="sxs-lookup"><span data-stu-id="6cf02-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="6cf02-104">Når du bruker denne funksjonen, konfigurerer automatisk koble til Azure AD synkroniseringsregler til:</span><span class="sxs-lookup"><span data-stu-id="6cf02-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="6cf02-105">Bruk msDS-ConsistencyGuid som sourceAnchor-attributt for brukerobjekter.</span><span class="sxs-lookup"><span data-stu-id="6cf02-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="6cf02-106">ObjectGUID brukes for andre objekttyper.</span><span class="sxs-lookup"><span data-stu-id="6cf02-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="6cf02-107">For en gitt lokale AD-bruker objektet der msDS-ConsistencyGuid-attributtet ikke er fylt ut på forhånd, Azure AD koble til skriver objectGUID verdien tilbake til msDS-ConsistencyGuid-attributtet i lokale Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6cf02-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="6cf02-108">Etter at attributtet msDS-ConsistencyGuid er fylt ut, eksporterer Azure AD-koble deretter objektet til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6cf02-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="6cf02-109">**Merk:** En gang en lokale AD-objektet er importert til Azure AD-tilkobling (som er, importeres til AD Connector plass og forventet i Metaverse), kan du ikke endre verdien sourceAnchor lenger.</span><span class="sxs-lookup"><span data-stu-id="6cf02-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="6cf02-110">Angi verdien for sourceAnchor for en gitt lokale AD objekt, konfigurere sin msDS-ConsistencyGuid-attributtet før den importeres til Azure AD-tilkobling.</span><span class="sxs-lookup"><span data-stu-id="6cf02-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="6cf02-111">Hvis du vil ha mer informasjon om SourceAnchor og ConsistencyGuid, se følgende: [Azure AD-tilkobling: utforme konsepter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="6cf02-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

