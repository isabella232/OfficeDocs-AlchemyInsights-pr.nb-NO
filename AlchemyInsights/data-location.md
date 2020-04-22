---
title: Dataplassering
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655291"
---
# <a name="data-location"></a><span data-ttu-id="60a10-102">Dataplassering</span><span class="sxs-lookup"><span data-stu-id="60a10-102">Data location</span></span>

<span data-ttu-id="60a10-103">Du kan vise plasseringen til leieren i administrasjonssenteret eller ved å koble til Exchange Online via PowerShell.</span><span class="sxs-lookup"><span data-stu-id="60a10-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="60a10-104">**Administrasjonssenter:**</span><span class="sxs-lookup"><span data-stu-id="60a10-104">**Admin center:**</span></span>
1. <span data-ttu-id="60a10-105">Logg på [administrasjonssenteret](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="60a10-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="60a10-106">Velg **Innstillinger** > **Organisasjonsprofil**.</span><span class="sxs-lookup"><span data-stu-id="60a10-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="60a10-107">Velg **Vis detaljer**under **Dataplassering**.</span><span class="sxs-lookup"><span data-stu-id="60a10-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="60a10-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="60a10-108">**PowerShell:**</span></span>
1. <span data-ttu-id="60a10-109">Koble til Exchange Online ved hjelp av Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="60a10-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="60a10-110">Utfør cmdleten [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) for å vise en liste over leierens egenskaper.</span><span class="sxs-lookup"><span data-stu-id="60a10-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="60a10-111">Se på egenskapen OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="60a10-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="60a10-112">Når du har dataplasseringen for EXO og SPO, kan du bestemme dataplasseringen for andre tjenester du kan bruke fra [Hvor dataene dine befinner seg.](https://products.office.com/where-is-your-data-located)</span><span class="sxs-lookup"><span data-stu-id="60a10-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>