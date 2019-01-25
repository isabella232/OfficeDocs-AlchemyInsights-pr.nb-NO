---
title: Kan ikke legge til en arbeidsflyt for godkjenning av 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: a83a9621ca0f7764d3f2c0a698dbffd80d55e80c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29482175"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="9dca0-102">Kan ikke legge til en arbeidsflyt for godkjenning av 2010</span><span class="sxs-lookup"><span data-stu-id="9dca0-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="9dca0-103">Du kan legge et globalt gjenbrukbar arbeidsflyt (for eksempel "godkjenning - SharePoint 2010") til lister eller biblioteker i en områdesamling for Microsoft SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9dca0-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="9dca0-104">Hvis du vil løse dette problemet, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="9dca0-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="9dca0-105">Åpne webområdet til roten av områdesamlingen i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="9dca0-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="9dca0-106">Under **Områdeobjekter**, velger du **arbeidsflyter**.</span><span class="sxs-lookup"><span data-stu-id="9dca0-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="9dca0-107">Velg **Gjenbrukbare arbeidsflyt**i **Ny** -delen av båndet **arbeidsflyter** .</span><span class="sxs-lookup"><span data-stu-id="9dca0-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="9dca0-p101">Angi navnet på skjemaet **Opprett gjenbrukbare arbeidsflyten** \*\* *Repair2010* \*\*. Klikk **SharePoint 2010 arbeidsflyt**for **Plattformen**, og klikk deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="9dca0-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="9dca0-110">Velg **Publiser**i delen **Lagre** **arbeidsflyt** -båndet.</span><span class="sxs-lookup"><span data-stu-id="9dca0-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="9dca0-p102">Velg **Publiser globalt**i delen **Behandle** **arbeidsflyt** -båndet. I bekreftelsesdialogboksen som vises, velger du **OK**.</span><span class="sxs-lookup"><span data-stu-id="9dca0-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="9dca0-p103">Finne webområdet til roten av områdesamlingen i en webleser, og deretter bruker du **Områdeinnstillinger** \> **Funksjoner i områdesamling**. Aktiver/deaktiver funksjonen **arbeidsflyter** :</span><span class="sxs-lookup"><span data-stu-id="9dca0-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="9dca0-115">· Hvis funksjonen er *aktivert* , klikker du **Deaktiver,** og klikk deretter **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="9dca0-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="9dca0-116">· Hvis funksjonen er *deaktivert* , klikker du **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="9dca0-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="9dca0-117">For mer informasjon kan du se følgende [artikkel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="9dca0-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

