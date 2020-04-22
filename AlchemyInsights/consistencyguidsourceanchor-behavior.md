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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="defac-102">ConsistencyGuid / sourceAnchor atferd</span><span class="sxs-lookup"><span data-stu-id="defac-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="defac-103">Azure AD Connect (versjon 1.1.524.0 og etter) forenkler nå bruken av msDS-ConsistencyGuid som sourceAnchor-attributt.</span><span class="sxs-lookup"><span data-stu-id="defac-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="defac-104">Når du bruker denne funksjonen, konfigurerer Azure AD Connect automatisk synkroniseringsreglene til:</span><span class="sxs-lookup"><span data-stu-id="defac-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="defac-105">Bruk msDS-ConsistencyGuid som sourceAnchor -attributtet for brukerobjekter.</span><span class="sxs-lookup"><span data-stu-id="defac-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="defac-106">ObjectGUID brukes for andre objekttyper.</span><span class="sxs-lookup"><span data-stu-id="defac-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="defac-107">For et gitt lokalt AD-brukerobjekt med msDS-ConsistencyGuid-attributtet ikke er fylt ut, skriver Azure AD Connect sin objectGUID-verdi tilbake til attributtet msDS-ConsistencyGuid i lokale Active Directory.</span><span class="sxs-lookup"><span data-stu-id="defac-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="defac-108">Når attributtet msDS-ConsistencyGuid er fylt ut, eksporterer Azure AD Connect objektet til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="defac-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="defac-109">**Merk:** Når et lokalt AD-objekt er importert til Azure AD Connect (det vil si importert til AD Connector Space og projisert til Metaverse), kan du ikke endre sourceAnchor-verdien lenger.</span><span class="sxs-lookup"><span data-stu-id="defac-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="defac-110">Hvis du vil angi sourceAnchor-verdien for et gitt lokalt AD-objekt, konfigurerer du attributtet msDS-ConsistencyGuid før det importeres til Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="defac-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="defac-111">Hvis du vil ha mer informasjon om SourceAnchor og ConsistencyGuid, kan du se følgende: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="defac-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

