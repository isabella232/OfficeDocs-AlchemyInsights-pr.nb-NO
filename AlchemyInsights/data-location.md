---
title: Data plassering
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
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627855"
---
# <a name="data-location"></a><span data-ttu-id="21a1f-102">Data plassering</span><span class="sxs-lookup"><span data-stu-id="21a1f-102">Data location</span></span>

<span data-ttu-id="21a1f-103">Du kan vise plasseringen av din Office 365 leier i administrasjonssenteret eller ved å koble til Exchange Online via PowerShell.</span><span class="sxs-lookup"><span data-stu-id="21a1f-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="21a1f-104">**Administrasjonssenter:**</span><span class="sxs-lookup"><span data-stu-id="21a1f-104">**Admin center:**</span></span>
1. <span data-ttu-id="21a1f-105">Logg på [administrasjonssenteret](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="21a1f-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="21a1f-106">Velg **Innstillinger** > **organisasjonsprofil**.</span><span class="sxs-lookup"><span data-stu-id="21a1f-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="21a1f-107">Velg **Vis detaljer**under **data plassering**.</span><span class="sxs-lookup"><span data-stu-id="21a1f-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="21a1f-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="21a1f-108">**PowerShell:**</span></span>
1. <span data-ttu-id="21a1f-109">Koble til Exchange Online ved hjelp av Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="21a1f-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="21a1f-110">Kjør cmdleten [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) for å vise en liste over egenskapene for leieren.</span><span class="sxs-lookup"><span data-stu-id="21a1f-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="21a1f-111">Se på OrganizationId-egenskapen.</span><span class="sxs-lookup"><span data-stu-id="21a1f-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="21a1f-112">Når du har data plasseringen for EXO og SPO, kan du bestemme data plasseringen for andre tjenester du kan bruke [der dataene er plassert](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="21a1f-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>