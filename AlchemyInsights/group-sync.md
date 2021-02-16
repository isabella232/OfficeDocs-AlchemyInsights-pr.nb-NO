---
title: Gruppesynkronisering
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256791"
---
# <a name="group-sync"></a><span data-ttu-id="3f55e-102">Gruppesynkronisering</span><span class="sxs-lookup"><span data-stu-id="3f55e-102">Group sync</span></span>

<span data-ttu-id="3f55e-103">Denne artikkelen gir veiledning om gruppesynkronisering.</span><span class="sxs-lookup"><span data-stu-id="3f55e-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="3f55e-104">Hvis en global administrator eller gruppeeier ikke kan endre gruppeegenskaper eller legge til medlemmer eller tilordne eiere i Azure Portal, må du kontrollere at myndighetskilden for gruppen er Azure Active Directory (Azure AD) for den globale administratoren eller gruppeeieren for å endre gruppen.</span><span class="sxs-lookup"><span data-stu-id="3f55e-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="3f55e-105">Før du prøver å slette en synkronisert gruppe i Azure AD, må du kontrollere at du har slettet alle tilordnede [lisenser](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) for å unngå feil.</span><span class="sxs-lookup"><span data-stu-id="3f55e-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="3f55e-106">Hvis du vil forstå hvordan du synkroniserer brukere, grupper og kontakter, kan du se [Azure AD Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)og følge synkronisering av en lokal gruppe til Azure ved hjelp av Azure AD Connect for å synkronisere [perm-grupper](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) ved hjelp av AD Connect.</span><span class="sxs-lookup"><span data-stu-id="3f55e-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="3f55e-107">Følg denne veiledningen [for feilsøking av feil under synkronisering](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) for å feilsøke vanlige feil under synkronisering.</span><span class="sxs-lookup"><span data-stu-id="3f55e-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

