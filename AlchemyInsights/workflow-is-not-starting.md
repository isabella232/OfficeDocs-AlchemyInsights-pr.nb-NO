---
title: Arbeids flyten starter ikke
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
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794776"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="82f98-102">Arbeids flyten starter ikke</span><span class="sxs-lookup"><span data-stu-id="82f98-102">Workflow is not starting</span></span>

- <span data-ttu-id="82f98-103">Arbeids flyter i SharePoint 2010 og SharePoint 2013 starter ikke.</span><span class="sxs-lookup"><span data-stu-id="82f98-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="82f98-104">Hvis arbeids flyten ikke starter, kan det være et midlertidig tjeneste problem der brukere kan oppleve uregelmessige forsinkelser med arbeids flyt frem drift.</span><span class="sxs-lookup"><span data-stu-id="82f98-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="82f98-105">Kontroller [instrument bordet for tjeneste tilstand](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) for å se om organisasjonen er berørt.</span><span class="sxs-lookup"><span data-stu-id="82f98-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="82f98-106">Hvis det har gått mer enn 24 timer siden du så dette problemet, kan du logge en støtte forespørsel.</span><span class="sxs-lookup"><span data-stu-id="82f98-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="82f98-107">I mange tilfeller arbeider vi allerede med en løsning.</span><span class="sxs-lookup"><span data-stu-id="82f98-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="82f98-108">Gi oss minst 24 timer til å fullføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="82f98-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="82f98-109">Arbeids flyter i SharePoint 2010 forsinket ved start.</span><span class="sxs-lookup"><span data-stu-id="82f98-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="82f98-110">Dette skjer hvis arbeids flyten utløses i store grupper.</span><span class="sxs-lookup"><span data-stu-id="82f98-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="82f98-111">(for eksempel når flere elementer legges til samtidig).</span><span class="sxs-lookup"><span data-stu-id="82f98-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="82f98-112">Arbeids flyter er ikke utformet for å kjøre i sanntid, så en forsinkelse er ved å utforme virke måte.</span><span class="sxs-lookup"><span data-stu-id="82f98-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="82f98-113">Hvis arbeids flyten er omfattende språk for Extensible Object Markup (XMOL), kan kompileringen ta lang tid.</span><span class="sxs-lookup"><span data-stu-id="82f98-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="82f98-114">Se [denne](https://support.microsoft.com//kb/3043697) artikkelen.</span><span class="sxs-lookup"><span data-stu-id="82f98-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="82f98-115">Du bør forenkle arbeids flyten eller utforme den på nytt ved hjelp av arbeids flyt plattform typen Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="82f98-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="82f98-116">Hvis arbeids flyt loggen er blitt stor, kan det være lurt å tømme elementene eller opprette en ny logg liste.</span><span class="sxs-lookup"><span data-stu-id="82f98-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="82f98-117">Mer informasjon: [Tøm arbeids flyt Logg](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="82f98-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="82f98-118">Beslektede emner</span><span class="sxs-lookup"><span data-stu-id="82f98-118">Related topics</span></span>
<span data-ttu-id="82f98-119">Vil du prøve Microsoft flyt inn i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="82f98-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="82f98-120">Opprett flyt</span><span class="sxs-lookup"><span data-stu-id="82f98-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="82f98-121">SharePoint og flyt</span><span class="sxs-lookup"><span data-stu-id="82f98-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


