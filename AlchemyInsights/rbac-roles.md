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
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923140"
---
# <a name="rbac-rules"></a>RBAC-regler

Hvis du får tillatelsesfeilen: 

- Klienten med objekt-ID har ikke tillatelse til å utføre handling **over omfanget (kode: AuthorizationFailed)**: Når du prøver å opprette en ressurs, kontrollerer du at du er logget på med en bruker som er tilordnet en rolle som har skrivetillatelse til ressursen i det valgte omfanget. Hvis du for eksempel vil administrere virtuelle maskiner [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) i en ressursgruppe, bør du ha rollen Som bidragsyter for virtuell maskin i ressursgruppen (eller overordnet omfang). Hvis du vil ha en liste over tillatelsene for hver innebygde rolle, kan du se [Innebygde roller for Azure-ressurser](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- Du har ikke tillatelse til å opprette en støtteforespørsel: Når du prøver å opprette eller oppdatere en støtteforespørsel, må du kontrollere at du er logget på med en bruker som er tilordnet en rolle som har tillatelsen Microsoft.Support/supportTickets/write, for eksempel Bidragsyter for støtteforespørsel [.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)
- Du kan ikke opprette flere rolletilordninger **(kode: RoleAssignmentLimitExceeded)**: Når du prøver å tilordne en rolle, kan du prøve å redusere antall rolletilordninger ved å tilordne roller til grupper i stedet. Azure støtter opptil **2000** rolletilordninger per abonnement.

Hvis du vil ha mer informasjon om Azure RBAC-roller, kan du se [Azure RBAC-roller](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
