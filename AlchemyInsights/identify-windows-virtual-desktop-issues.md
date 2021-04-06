---
title: Identifisere problemer med virtuelt skrivebord i Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595854"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Identifisere problemer med virtuelt skrivebord i Windows

Windows Virtual Desktop Diagnostics bruker bare én PowerShell-cmdlet, men inneholder mange valgfrie parametere for å begrense og isolere problemer. Slik kommer du i gang: 

1. Last ned og importer Windows Virtual Desktop PowerShell-modulen. Hvis du vil ha mer informasjon, [kan du se Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).

1. Kjør følgende cmdlet for å logge på kontoen din:
    
    Eksempel: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**OBS!** Alle spørringer som bruker PowerShell, må inneholde parameterne -UserName eller -ActivityID. Hvis du vil ha informasjon om overvåkingsfunksjoner, kan du se Bruke [Log Analytics for diagnosefunksjonen.](https://go.microsoft.com/fwlink/?linkid=2126847)

Hvis du vil filtrere diagnoseaktiviteter etter bruker, kjører du følgende cmdlet:

Eksempel: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Det finnes en liste over filtre du kan kjøre for å diagnostisere problemer. Hvis du vil lære mer om diagnostisering av problemer, kan du se [Identifisere og diagnostisere problemer med Virtuelt skrivebord i Windows.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

Hvis du vil lære mer om vanlige feil, kan du se [Vanlige feil senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
