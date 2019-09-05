---
title: Manglende arbeidsflyt ble ikke aktivert
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753805"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="10955-102">Manglende arbeidsflyt ble ikke aktivert</span><span class="sxs-lookup"><span data-stu-id="10955-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="10955-103">I en områdesamling for Microsoft SharePoint kan du ikke legge til en globalt gjenbrukbar arbeidsflyt (for eksempel "godkjenning – SharePoint 2010") i en liste eller et bibliotek.</span><span class="sxs-lookup"><span data-stu-id="10955-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="10955-104">Hvis du vil løse dette problemet, følger du denne fremgangsmåten:</span><span class="sxs-lookup"><span data-stu-id="10955-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="10955-105">Åpne det primære webområdet for områdesamlingen i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="10955-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="10955-106">Velg **arbeidsflyter**under **områdeobjekter**.</span><span class="sxs-lookup"><span data-stu-id="10955-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="10955-107">Velg **gjenbrukbar arbeidsflyt**i den **nye** delen av båndet **arbeidsflyter** .</span><span class="sxs-lookup"><span data-stu-id="10955-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="10955-108">I skjemaet **Opprett gjenbrukbar arbeidsflyt** skriver du inn navnet \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="10955-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="10955-109">For **plattform type**, klikker du **SharePoint 2010 arbeidsflyt**, og klikk deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="10955-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="10955-110">Velg **Publiser**i **Lagre** -delen av **arbeidsflyt** båndet.</span><span class="sxs-lookup"><span data-stu-id="10955-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="10955-111">Velg **Publiser globalt**i **Behandle** -delen av **arbeidsflyt** båndet.</span><span class="sxs-lookup"><span data-stu-id="10955-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="10955-112">Velg **OK**i bekreftelsesdialogboksen som vises.</span><span class="sxs-lookup"><span data-stu-id="10955-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="10955-113">I en webleser finner du rotwebområdet for områdesamlingen, og deretter får du tilgang til **områdesamlingsfunksjoner** **for områdeinnstillinger** \> .</span><span class="sxs-lookup"><span data-stu-id="10955-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="10955-114">Deretter aktiverer du funksjonen **arbeidsflyter** :</span><span class="sxs-lookup"><span data-stu-id="10955-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="10955-115">· Hvis funksjonen er *aktivert* , klikker du **Deaktiver,** og klikk deretter **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="10955-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="10955-116">· Hvis funksjonen er *deaktivert* , klikker du **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="10955-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="10955-117">For mer informasjon henvises til følgende [artikkel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="10955-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

