---
title: Arbeidsflyten starter ikke
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766106"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="13970-102">Arbeidsflyten starter ikke</span><span class="sxs-lookup"><span data-stu-id="13970-102">Workflow is not starting</span></span>

- <span data-ttu-id="13970-103">SharePoint 2010- og SharePoint 2013-arbeidsflyter starter ikke.</span><span class="sxs-lookup"><span data-stu-id="13970-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="13970-104">Hvis arbeidsflyten ikke starter, kan det være et midlertidig tjenesteproblem der brukere kan oppleve periodiske forsinkelser med arbeidsflytfremdriften.</span><span class="sxs-lookup"><span data-stu-id="13970-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="13970-105">Kontroller [instrumentbordet for servicetilstand](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) for å se om organisasjonen påvirkes.</span><span class="sxs-lookup"><span data-stu-id="13970-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="13970-106">Hvis det har gått mer enn 24 timer siden du først så dette problemet, kan du logge en støttebillett.</span><span class="sxs-lookup"><span data-stu-id="13970-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="13970-107">I mange tilfeller jobber vi allerede med en løsning.</span><span class="sxs-lookup"><span data-stu-id="13970-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="13970-108">Vennligst gi oss minst 24 timer for å fullføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="13970-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="13970-109">SharePoint 2010 arbeidsflyter forsinket ved start.</span><span class="sxs-lookup"><span data-stu-id="13970-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="13970-110">Dette skjer hvis arbeidsflyten utløses i store partier.</span><span class="sxs-lookup"><span data-stu-id="13970-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="13970-111">(for eksempel når flere elementer legges til samtidig).</span><span class="sxs-lookup"><span data-stu-id="13970-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="13970-112">Arbeidsflyter er ikke utformet for å kjøre sanntid, så en forsinkelse er etter utformingsvirkemåte.</span><span class="sxs-lookup"><span data-stu-id="13970-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="13970-113">Hvis arbeidsflyten er kompleks xmol (Extensible Object Markup Language), kan kompilering være treg.</span><span class="sxs-lookup"><span data-stu-id="13970-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="13970-114">Sjekk [denne](https://support.microsoft.com//kb/3043697) artikkelen.</span><span class="sxs-lookup"><span data-stu-id="13970-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="13970-115">Du bør forenkle arbeidsflyten eller utforme den på nytt ved hjelp av microsoft SharePoint 2013 arbeidsflytplattformtypen.</span><span class="sxs-lookup"><span data-stu-id="13970-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="13970-116">Hvis arbeidsflytloggen har blitt stor, kan det være lurt å tømme elementene eller opprette en ny loggliste.</span><span class="sxs-lookup"><span data-stu-id="13970-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="13970-117">Mer informasjon : [Tøm arbeidsflytloggen](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="13970-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="13970-118">Beslektede emner</span><span class="sxs-lookup"><span data-stu-id="13970-118">Related topics</span></span>
<span data-ttu-id="13970-119">Vil du prøve Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="13970-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="13970-120">Opprett flyt</span><span class="sxs-lookup"><span data-stu-id="13970-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="13970-121">SharePoint og Flow</span><span class="sxs-lookup"><span data-stu-id="13970-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


