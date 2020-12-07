---
title: 'RBAC-roller '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583947"
---
# <a name="rbac-rules"></a><span data-ttu-id="ddce0-102">RBAC-regler</span><span class="sxs-lookup"><span data-stu-id="ddce0-102">RBAC rules</span></span>

<span data-ttu-id="ddce0-103">Hvis du får tillatelses feilen:</span><span class="sxs-lookup"><span data-stu-id="ddce0-103">If you get the permission error:</span></span> 

- <span data-ttu-id="ddce0-104">**Klienten med objekt-ID har ikke autorisasjon til å utføre handlinger over omfang (kode: AuthorizationFailed)**: Når du prøver å opprette en ressurs, må du kontrollere at du for øyeblikket er logget på med en bruker som er tilordnet en rolle som har skrive tillatelse til ressursen i det valgte området.</span><span class="sxs-lookup"><span data-stu-id="ddce0-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="ddce0-105">Hvis du for eksempel vil administrere virtuelle maskiner i en ressurs gruppe, må du ha rollen som [bidrags yter for virtuell maskin](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) på ressurs gruppen (eller overordnet omfang).</span><span class="sxs-lookup"><span data-stu-id="ddce0-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="ddce0-106">Hvis du vil ha en liste over tillatelsene for hver innebygd rolle, kan du se [innebygde roller for Azure-ressurser](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ddce0-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="ddce0-107">**Du har ikke tillatelse til å opprette en støtte anmodning**: Når du prøver å opprette eller oppdatere en støtte kvittering, må du kontrollere at du for øyeblikket er logget på med en bruker som er tilordnet en rolle som har Microsoft. støtte/supportTickets/Write-tillatelse, for eksempel [bidrags yter for støtte anmodning](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="ddce0-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="ddce0-108">Du **kan ikke opprette flere rolle tilordninger (kode: RoleAssignmentLimitExceeded)**: Når du prøver å tilordne en rolle, må du prøve å redusere antallet rolle tilordninger ved å tilordne roller til grupper i stedet.</span><span class="sxs-lookup"><span data-stu-id="ddce0-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="ddce0-109">Azure støtter opptil **2000** rolle tilordninger per abonnement.</span><span class="sxs-lookup"><span data-stu-id="ddce0-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="ddce0-110">Hvis du vil ha mer informasjon om Azure RBAC-roller, kan du se [Azure RBAC Roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ddce0-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
