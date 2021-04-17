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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="76a9d-102">KonsekvensGuid/ sourceAnchor-virkemåte</span><span class="sxs-lookup"><span data-stu-id="76a9d-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="76a9d-103">Azure AD Connect (versjon 1.1.524.0 og etter) forenkler nå bruken av msDS-ConsistencyGuid som sourceAnchor-attributt.</span><span class="sxs-lookup"><span data-stu-id="76a9d-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="76a9d-104">Når du bruker denne funksjonen, konfigurerer Azure AD Connect automatisk synkroniseringsreglene til å:</span><span class="sxs-lookup"><span data-stu-id="76a9d-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="76a9d-105">Bruk msDS-ConsistencyGuid som sourceAnchor-attributt for brukerobjekter.</span><span class="sxs-lookup"><span data-stu-id="76a9d-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="76a9d-106">ObjectGUID brukes for andre objekttyper.</span><span class="sxs-lookup"><span data-stu-id="76a9d-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="76a9d-107">For et gitt lokalt AD User-objekt der msDS-ConsistencyGuid-attributtet ikke er fylt ut, skriver Azure AD Connect objektGUID-verdien tilbake til msDS-ConsistencyGuid-attributtet i lokal Active Directory.</span><span class="sxs-lookup"><span data-stu-id="76a9d-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="76a9d-108">Når msDS-ConsistencyGuid-attributtet er fylt ut, eksporterer Azure AD Connect deretter objektet til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="76a9d-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="76a9d-109">**Obs!** Når et lokalt AD-objekt er importert til Azure AD Connect (det vil si importert til AD Connector Space og projiseres til Metaverse), kan du ikke endre sourceAnchor-verdien lenger.</span><span class="sxs-lookup"><span data-stu-id="76a9d-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="76a9d-110">Hvis du vil angi sourceAnchor-verdien for et gitt lokalt AD-objekt, konfigurerer du attributtet msDS-ConsistencyGuid før det importeres til Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="76a9d-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="76a9d-111">Hvis du vil ha mer informasjon om SourceAnchor og Konsekvensguid, kan du se følgende: [Azure AD Connect: Utformingskonsepter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="76a9d-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

