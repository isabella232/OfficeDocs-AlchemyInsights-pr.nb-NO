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
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="e01a3-102">Identifisere problemer med virtuelt skrivebord i Windows</span><span class="sxs-lookup"><span data-stu-id="e01a3-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="e01a3-103">Windows Virtual Desktop Diagnostics bruker bare én PowerShell-cmdlet, men inneholder mange valgfrie parametere for å begrense og isolere problemer.</span><span class="sxs-lookup"><span data-stu-id="e01a3-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="e01a3-104">Slik kommer du i gang:</span><span class="sxs-lookup"><span data-stu-id="e01a3-104">To get started:</span></span> 

1. <span data-ttu-id="e01a3-105">Last ned og importer Windows Virtual Desktop PowerShell-modulen.</span><span class="sxs-lookup"><span data-stu-id="e01a3-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="e01a3-106">Hvis du vil ha mer informasjon, [kan du se Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span><span class="sxs-lookup"><span data-stu-id="e01a3-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="e01a3-107">Kjør følgende cmdlet for å logge på kontoen din:</span><span class="sxs-lookup"><span data-stu-id="e01a3-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="e01a3-108">Eksempel: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="e01a3-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="e01a3-109">**OBS!** Alle spørringer som bruker PowerShell, må inneholde parameterne -UserName eller -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="e01a3-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="e01a3-110">Hvis du vil ha informasjon om overvåkingsfunksjoner, kan du se Bruke [Log Analytics for diagnosefunksjonen.](https://go.microsoft.com/fwlink/?linkid=2126847)</span><span class="sxs-lookup"><span data-stu-id="e01a3-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="e01a3-111">Hvis du vil filtrere diagnoseaktiviteter etter bruker, kjører du følgende cmdlet:</span><span class="sxs-lookup"><span data-stu-id="e01a3-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="e01a3-112">Eksempel: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="e01a3-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="e01a3-113">Det finnes en liste over filtre du kan kjøre for å diagnostisere problemer.</span><span class="sxs-lookup"><span data-stu-id="e01a3-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="e01a3-114">Hvis du vil lære mer om diagnostisering av problemer, kan du se [Identifisere og diagnostisere problemer med Virtuelt skrivebord i Windows.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="e01a3-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="e01a3-115">Hvis du vil lære mer om vanlige feil, kan du se [Vanlige feil senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="e01a3-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
