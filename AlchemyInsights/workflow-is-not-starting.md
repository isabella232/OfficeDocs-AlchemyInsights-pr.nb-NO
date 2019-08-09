---
title: Arbeidsflyten starter ikke
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: a3bac74c19a77b7703f948c1d8b6bcd182e9b075
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270789"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="03096-102">Arbeidsflyten starter ikke</span><span class="sxs-lookup"><span data-stu-id="03096-102">Workflow is not starting</span></span>

- <span data-ttu-id="03096-103">Arbeidsflyter for SharePoint 2010 og SharePoint 2013 starter ikke.</span><span class="sxs-lookup"><span data-stu-id="03096-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="03096-104">Hvis arbeidsflyten ikke starter, kan det være et problem med midlertidig tjeneste der brukere kan oppleve periodiske forsinkelser med arbeidsflyten pågår.</span><span class="sxs-lookup"><span data-stu-id="03096-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="03096-105">Kontroller [Service helse instrumentbord](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) for å se Hvis din organisasjon er påvirket.</span><span class="sxs-lookup"><span data-stu-id="03096-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="03096-106">Hvis det har gått mer enn 24 timer etter at du først så dette problemet, logger du deg en support billett.</span><span class="sxs-lookup"><span data-stu-id="03096-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="03096-107">I mange tilfeller kan arbeider vi allerede med en løsning.</span><span class="sxs-lookup"><span data-stu-id="03096-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="03096-108">Gi oss minst 24 timer å fullføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="03096-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="03096-109">SharePoint 2010-arbeidsflyter forsinket på start.</span><span class="sxs-lookup"><span data-stu-id="03096-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="03096-110">Dette skjer hvis arbeidsflyten utløses i store grupper.</span><span class="sxs-lookup"><span data-stu-id="03096-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="03096-111">(for eksempel når flere elementer er lagt til på en gang).</span><span class="sxs-lookup"><span data-stu-id="03096-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="03096-112">Arbeidsflyter er ikke utformet for å kjøre i sanntid, slik at en forsinkelse er standard virkemåte.</span><span class="sxs-lookup"><span data-stu-id="03096-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="03096-113">Hvis arbeidsflyten er komplekse Extensible Object Markup Language (XMOL), kan det ta lang tid kompilering.</span><span class="sxs-lookup"><span data-stu-id="03096-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="03096-114">Merk av i [denne](https://support.microsoft.com/en-us/kb/3043697) artikkelen.</span><span class="sxs-lookup"><span data-stu-id="03096-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    - <span data-ttu-id="03096-115">Du må forenkle arbeidsflyten diagramstørrelsen eller ved hjelp av Microsoft SharePoint 2013 plattform arbeidsflyttypen.</span><span class="sxs-lookup"><span data-stu-id="03096-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="03096-116">Hvis din Arbeidsflytlogg er blitt stor, kanskje du vil tømme varene eller opprette en ny loggliste.</span><span class="sxs-lookup"><span data-stu-id="03096-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="03096-117">Mer informasjon: [Tøm Arbeidsflytlogg](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="03096-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="03096-118">Beslektede emner</span><span class="sxs-lookup"><span data-stu-id="03096-118">Related topics</span></span>
<span data-ttu-id="03096-119">Vil du prøve Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="03096-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="03096-120">Opprette flyt</span><span class="sxs-lookup"><span data-stu-id="03096-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="03096-121">SharePoint og flyt</span><span class="sxs-lookup"><span data-stu-id="03096-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


