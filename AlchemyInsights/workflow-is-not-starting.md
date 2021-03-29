---
title: Arbeidsflyten starter ikke
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403752"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="20203-102">Arbeidsflyten starter ikke</span><span class="sxs-lookup"><span data-stu-id="20203-102">Workflow is not starting</span></span>

- <span data-ttu-id="20203-103">SharePoint 2010- og SharePoint 2013-arbeidsflyter starter ikke.</span><span class="sxs-lookup"><span data-stu-id="20203-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="20203-104">Hvis arbeidsflyten ikke starter, kan det være et midlertidig tjenesteproblem der brukere kan oppleve uregelmessig forsinkelser med arbeidsflytfremdriften.</span><span class="sxs-lookup"><span data-stu-id="20203-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="20203-105">Kontroller [instrumentbordet for tjenestetilstand](https://admin.microsoft.com/AdminPortal/Home/servicehealth) for å se om organisasjonen påvirkes.</span><span class="sxs-lookup"><span data-stu-id="20203-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="20203-106">Hvis det har gått mer enn 24 timer siden du så dette problemet, logger du en støtteforespørsel.</span><span class="sxs-lookup"><span data-stu-id="20203-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="20203-107">I mange tilfeller arbeider vi allerede med en løsning.</span><span class="sxs-lookup"><span data-stu-id="20203-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="20203-108">Gi oss minst 24 timer for å fullføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="20203-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="20203-109">SharePoint 2010-arbeidsflyter forsinket ved start.</span><span class="sxs-lookup"><span data-stu-id="20203-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="20203-110">Dette skjer hvis arbeidsflyten utløses i store grupper.</span><span class="sxs-lookup"><span data-stu-id="20203-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="20203-111">(for eksempel når flere elementer legges til samtidig).</span><span class="sxs-lookup"><span data-stu-id="20203-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="20203-112">Arbeidsflyter er ikke utformet for å kjøre i sanntid, så en forsinkelse er virkemåten til utformingen.</span><span class="sxs-lookup"><span data-stu-id="20203-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="20203-113">Hvis arbeidsflyten er kompleks extensible Object Markup Language (XMOL), kan kompileringen gå tregt.</span><span class="sxs-lookup"><span data-stu-id="20203-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="20203-114">Se [denne](https://support.microsoft.com//kb/3043697) artikkelen.</span><span class="sxs-lookup"><span data-stu-id="20203-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="20203-115">Du bør forenkle arbeidsflyten eller utforme den på nytt ved hjelp av plattformtypen Microsoft SharePoint 2013-arbeidsflyt.</span><span class="sxs-lookup"><span data-stu-id="20203-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="20203-116">Hvis arbeidsflytloggen har blitt stor, vil du kanskje fjerne elementene eller opprette en ny loggliste.</span><span class="sxs-lookup"><span data-stu-id="20203-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="20203-117">Mer informasjon: [Tømme arbeidsflytloggen](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="20203-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="20203-118">Beslektede emner</span><span class="sxs-lookup"><span data-stu-id="20203-118">Related topics</span></span>
<span data-ttu-id="20203-119">Vil du prøve Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="20203-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="20203-120">Opprette flyt</span><span class="sxs-lookup"><span data-stu-id="20203-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="20203-121">SharePoint og Flow</span><span class="sxs-lookup"><span data-stu-id="20203-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
