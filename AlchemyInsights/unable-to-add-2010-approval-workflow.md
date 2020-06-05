---
title: Kan ikke legge til arbeidsflyt for godkjenning av 2010
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: f40716dd399fe7bea1b606cd725676268dc0a66d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582856"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="5ad08-102">Kan ikke legge til arbeidsflyt for godkjenning av 2010</span><span class="sxs-lookup"><span data-stu-id="5ad08-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="5ad08-103">I en Microsoft SharePoint-områdesamling kan du ikke legge til en arbeidsflyt som kan brukes på nytt (for eksempel "Godkjenning - SharePoint 2010") i en liste eller et bibliotek.</span><span class="sxs-lookup"><span data-stu-id="5ad08-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="5ad08-104">Hvis du vil løse dette problemet, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="5ad08-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="5ad08-105">Åpne rotwebområdet for områdesamlingen i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="5ad08-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="5ad08-106">Velg **Arbeidsflyter**under **Områdeobjekter**.</span><span class="sxs-lookup"><span data-stu-id="5ad08-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="5ad08-107">Velg Arbeidsflyt som kan brukes på nytt, i **Ny-delen** på **Arbeidsflyter-båndet.** **Workflows**</span><span class="sxs-lookup"><span data-stu-id="5ad08-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="5ad08-108">I skjemaet **Opprett arbeidsflyt som kan brukes på nytt,** skriver du inn navnet \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="5ad08-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="5ad08-109">Klikk Arbeidsflyt for **SharePoint 2010**for **Plattformtype**, og klikk deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="5ad08-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="5ad08-110">Velg **Publiser**under **Lagre** på **Arbeidsflyt-båndet.**</span><span class="sxs-lookup"><span data-stu-id="5ad08-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="5ad08-111">Velg **Publiser globalt i** **Behandle-delen** på **Arbeidsflyt-båndet.**</span><span class="sxs-lookup"><span data-stu-id="5ad08-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="5ad08-112">Velg **OK**i bekreftelsesdialogboksen som vises.</span><span class="sxs-lookup"><span data-stu-id="5ad08-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="5ad08-113">Finn rotnettstedet for områdesamlingen i en nettleser, **Site Settings** og få deretter tilgang til \> **funksjoner for områdeinnstillinger områdesamling**.</span><span class="sxs-lookup"><span data-stu-id="5ad08-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="5ad08-114">Aktiver/deaktiver **arbeidsflytfunksjonen:**</span><span class="sxs-lookup"><span data-stu-id="5ad08-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="5ad08-115">· Hvis funksjonen er *Aktivert* , klikker du **Deaktiver,** og klikk deretter **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="5ad08-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="5ad08-116">· Hvis funksjonen er *Deaktivert* , klikker du **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="5ad08-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="5ad08-117">Hvis du vil ha mer informasjon, kan du se følgende [artikkel.](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="5ad08-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

