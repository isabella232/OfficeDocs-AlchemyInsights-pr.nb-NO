---
title: Domain service-synkronisering
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885569"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="e7d6f-102">Domain service-synkronisering</span><span class="sxs-lookup"><span data-stu-id="e7d6f-102">Domain service synchronization</span></span>

<span data-ttu-id="e7d6f-103">Objekter og legitimasjoner i et forvaltet Active Directory Domain Services-domene (Azure AD DS) kan enten opprettes lokalt i domenet, eller synkroniseres fra en Azure Active Directory-Tenant (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="e7d6f-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="e7d6f-104">Når du først distribuerer Azure AD DS, konfigureres en automatisk en veis synkronisering og startes for å rep likere objektene fra Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e7d6f-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="e7d6f-105">Denne en veis synkroniseringen fortsetter å kjøre i bakgrunnen for å holde det administrerte Azure AD DS-domenet oppdatert med eventuelle endringer fra Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e7d6f-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="e7d6f-106">Ingen synkronisering skjer fra Azure AD DS tilbake til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e7d6f-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="e7d6f-107">Hvis du vil ha mer informasjon om Azure Active Directory Domain service-synkronisering, kan du se [synkronisering av domene tjenester](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span><span class="sxs-lookup"><span data-stu-id="e7d6f-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
