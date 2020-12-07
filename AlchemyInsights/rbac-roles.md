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
# <a name="rbac-rules"></a>RBAC-regler

Hvis du får tillatelses feilen: 

- **Klienten med objekt-ID har ikke autorisasjon til å utføre handlinger over omfang (kode: AuthorizationFailed)**: Når du prøver å opprette en ressurs, må du kontrollere at du for øyeblikket er logget på med en bruker som er tilordnet en rolle som har skrive tillatelse til ressursen i det valgte området. Hvis du for eksempel vil administrere virtuelle maskiner i en ressurs gruppe, må du ha rollen som [bidrags yter for virtuell maskin](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) på ressurs gruppen (eller overordnet omfang). Hvis du vil ha en liste over tillatelsene for hver innebygd rolle, kan du se [innebygde roller for Azure-ressurser](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **Du har ikke tillatelse til å opprette en støtte anmodning**: Når du prøver å opprette eller oppdatere en støtte kvittering, må du kontrollere at du for øyeblikket er logget på med en bruker som er tilordnet en rolle som har Microsoft. støtte/supportTickets/Write-tillatelse, for eksempel [bidrags yter for støtte anmodning](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- Du **kan ikke opprette flere rolle tilordninger (kode: RoleAssignmentLimitExceeded)**: Når du prøver å tilordne en rolle, må du prøve å redusere antallet rolle tilordninger ved å tilordne roller til grupper i stedet. Azure støtter opptil **2000** rolle tilordninger per abonnement.

Hvis du vil ha mer informasjon om Azure RBAC-roller, kan du se [Azure RBAC Roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
