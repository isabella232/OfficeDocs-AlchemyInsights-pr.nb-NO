---
title: Kan ikke legge til standard godkjenningsarbeidsflyt i 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28302511"
---
# <a name="cant-add-default-2010-approval-workflow"></a><span data-ttu-id="f7d6e-102">Kan ikke legge til standard godkjenningsarbeidsflyt i 2010</span><span class="sxs-lookup"><span data-stu-id="f7d6e-102">Can't add default 2010 Approval Workflow</span></span>

<span data-ttu-id="f7d6e-103">Du kan legge et globalt gjenbrukbar arbeidsflyt (for eksempel "godkjenning - SharePoint 2010") til lister eller biblioteker i en områdesamling for Microsoft SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f7d6e-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="f7d6e-104">Hvis du vil løse dette problemet, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="f7d6e-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="f7d6e-105">Åpne webområdet til roten av områdesamlingen i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="f7d6e-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="f7d6e-106">Under **Områdeobjekter**, velger du **arbeidsflyter**.</span><span class="sxs-lookup"><span data-stu-id="f7d6e-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="f7d6e-107">Velg **Gjenbrukbare arbeidsflyt**i **Ny** -delen av båndet **arbeidsflyter** .</span><span class="sxs-lookup"><span data-stu-id="f7d6e-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="f7d6e-p101">Angi navnet på skjemaet **Opprett gjenbrukbare arbeidsflyten** \* \*\*Repair2010\*\*\*. Velg **SharePoint 2010 arbeidsflyt**for **Plattformen**, og velg deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="f7d6e-p101">On the **Create Reusable Workflow** form, enter the name  \* **Repair2010**\* . For **Platform Type**, select **SharePoint 2010 Workflow**, and then select **OK**.</span></span> 
  
5. <span data-ttu-id="f7d6e-110">Velg **Publiser**i delen **Lagre** **arbeidsflyt** -båndet.</span><span class="sxs-lookup"><span data-stu-id="f7d6e-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
6. <span data-ttu-id="f7d6e-p102">Velg **Publiser globalt**i delen **Behandle** **arbeidsflyt** -båndet. I bekreftelsesdialogboksen som vises, velger du **OK**.</span><span class="sxs-lookup"><span data-stu-id="f7d6e-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
7. <span data-ttu-id="f7d6e-p103">Finne webområdet til roten av områdesamlingen i en webleser, og deretter bruker du **Områdeinnstillinger** \> **Funksjoner i områdesamling**. Deretter Aktiver/deaktiver funksjonen **arbeidsflyter** :</span><span class="sxs-lookup"><span data-stu-id="f7d6e-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="f7d6e-115">· Hvis funksjonen er *aktivert* , klikker du **Deaktiver,** og klikk deretter **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="f7d6e-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="f7d6e-116">· Hvis funksjonen er *deaktivert* , klikker du **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="f7d6e-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="f7d6e-117">For mer informasjon kan du se følgende [artikkel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="f7d6e-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

