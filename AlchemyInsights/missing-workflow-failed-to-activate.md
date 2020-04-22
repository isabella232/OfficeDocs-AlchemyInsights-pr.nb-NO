---
title: Manglende arbeidsflyt kan ikke aktiveres
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762110"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="06661-102">Manglende arbeidsflyt kan ikke aktiveres</span><span class="sxs-lookup"><span data-stu-id="06661-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="06661-103">I en Microsoft SharePoint-områdesamling kan du ikke legge til en globalt gjenbrukbar arbeidsflyt (for eksempel "Godkjenning - SharePoint 2010") i en liste eller et bibliotek.</span><span class="sxs-lookup"><span data-stu-id="06661-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="06661-104">Hvis du vil løse dette problemet, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="06661-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="06661-105">Åpne rotwebområdet for områdesamlingen i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="06661-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="06661-106">Velg **Arbeidsflyter**under **Områdeobjekter**.</span><span class="sxs-lookup"><span data-stu-id="06661-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="06661-107">Velg **Arbeidsflyt** som **Workflows** **kan brukes på nytt**.</span><span class="sxs-lookup"><span data-stu-id="06661-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="06661-108">I skjemaet **Opprett ny brukbar arbeidsflyt** skriver du inn navnet \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="06661-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="06661-109">Klikk **SharePoint 2010-arbeidsflyt**for **Plattformtype**, og klikk deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="06661-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="06661-110">Velg **Publiser**i **Lagre-delen** på **Arbeidsflyt-båndet.**</span><span class="sxs-lookup"><span data-stu-id="06661-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="06661-111">Velg **Publiser globalt**i **Behandle-delen** på **Arbeidsflyt-båndet.**</span><span class="sxs-lookup"><span data-stu-id="06661-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="06661-112">Velg **OK**i bekreftelsesdialogboksen som vises.</span><span class="sxs-lookup"><span data-stu-id="06661-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="06661-113">Finn rotwebområdet for områdesamlingen i en nettleser, og få deretter tilgang til funksjoner **for områdeinnstillinger** \> **områdesamling**.</span><span class="sxs-lookup"><span data-stu-id="06661-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="06661-114">Deretter veksler du **arbeidsflytfunksjonen:**</span><span class="sxs-lookup"><span data-stu-id="06661-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="06661-115">· Hvis funksjonen er *Aktivert* , klikker du **Deaktiver,** og deretter klikker du **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="06661-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="06661-116">· Hvis funksjonen er *Deaktivert* , klikker du **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="06661-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="06661-117">Hvis du vil ha mer informasjon, kan du se følgende [artikkel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="06661-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

