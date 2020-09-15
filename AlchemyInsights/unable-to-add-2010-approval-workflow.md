---
title: Kan ikke legge til arbeids flyten for 2010-godkjenning
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699744"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="10f8a-102">Kan ikke legge til arbeids flyten for 2010-godkjenning</span><span class="sxs-lookup"><span data-stu-id="10f8a-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="10f8a-103">I en Microsoft SharePoint-områdesamling kan du ikke legge til en global gjenbrukbar arbeids flyt (for eksempel "godkjenning-SharePoint 2010") i en liste eller et bibliotek.</span><span class="sxs-lookup"><span data-stu-id="10f8a-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="10f8a-104">Følg denne Fremgangs måten for å løse dette problemet:</span><span class="sxs-lookup"><span data-stu-id="10f8a-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="10f8a-105">Åpne rot nettstedet for nettsteds samlingen i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="10f8a-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="10f8a-106">Velg **arbeids flyter**under **område objekter**.</span><span class="sxs-lookup"><span data-stu-id="10f8a-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="10f8a-107">Velg **gjenbrukbar arbeids flyt**i den **nye** delen av **arbeids flyt** båndet.</span><span class="sxs-lookup"><span data-stu-id="10f8a-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="10f8a-108">Skriv inn navnet \* \* *Repair2010* \* \* i skjemaet **Opprett gjenbrukbar arbeids flyt** .</span><span class="sxs-lookup"><span data-stu-id="10f8a-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="10f8a-109">For **plattform type**klikker du **SharePoint 2010-arbeidsflyt**, og deretter klikker du **OK**.</span><span class="sxs-lookup"><span data-stu-id="10f8a-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="10f8a-110">Velg **Publiser**i **Lagre** -delen på **arbeids flyt** båndet.</span><span class="sxs-lookup"><span data-stu-id="10f8a-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="10f8a-111">Velg **Publiser globalt**i delen **Behandle** i **arbeids flyt** båndet.</span><span class="sxs-lookup"><span data-stu-id="10f8a-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="10f8a-112">Velg **OK**i bekreftelses dialog boksen som vises.</span><span class="sxs-lookup"><span data-stu-id="10f8a-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="10f8a-113">Finn rot nettstedet for nettsteds samlingen i en nett leser, og få deretter tilgang **Site Settings** til område \> **samlings funksjoner**for nettsteds innstillinger.</span><span class="sxs-lookup"><span data-stu-id="10f8a-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="10f8a-114">Aktivere/deaktivere funksjonen **arbeids flyter** :</span><span class="sxs-lookup"><span data-stu-id="10f8a-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="10f8a-115">· Hvis funksjonen er  *aktivert*  , klikker du **Deaktiver,** og deretter klikker du **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="10f8a-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="10f8a-116">· Hvis funksjonen er  *deaktivert*  , klikker du **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="10f8a-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="10f8a-117">Hvis du vil ha mer informasjon, kan du se følgende [artikkel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="10f8a-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

