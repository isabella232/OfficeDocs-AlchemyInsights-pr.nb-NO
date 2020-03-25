---
title: Problemer under overføring av data til SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "1885"
ms.openlocfilehash: b53a98480bab48497274c7358f7e606caa477f5a
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931703"
---
# <a name="issues-while-migrating-data-to-sharepoint-online"></a><span data-ttu-id="e06fb-102">Problemer under overføring av data til SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="e06fb-102">Issues while migrating data to SharePoint Online</span></span>

<span data-ttu-id="e06fb-103">**Viktig:** Mange SharePoint Online- og OneDrive-kunder kjører forretningskritiske programmer mot tjenesten som kjører i bakgrunnen.</span><span class="sxs-lookup"><span data-stu-id="e06fb-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="e06fb-104">Disse inkluderer innholdsoverføring, Hindring av tap av data (DLP) og sikkerhetskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="e06fb-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="e06fb-105">I løpet av disse enestående tider tar vi skritt for å sikre at SharePoint Online- og OneDrive-tjenester forblir svært tilgjengelige og pålitelige for brukerne som er avhengige av tjenesten mer enn noensinne i scenarier for eksternt arbeid.</span><span class="sxs-lookup"><span data-stu-id="e06fb-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="e06fb-106">Til støtte for dette målet har vi implementert strammere reguleringsgrenser for bakgrunnsapper (overførings-, DLP- og sikkerhetskopieringsløsninger) i løpet av ukedagsdagstimene.</span><span class="sxs-lookup"><span data-stu-id="e06fb-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="e06fb-107">Du bør forvente at disse appene vil oppnå svært begrenset gjennomstrømning i disse tider.</span><span class="sxs-lookup"><span data-stu-id="e06fb-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="e06fb-108">I løpet av kvelds- og helgetiden for regionen vil tjenesten imidlertid være klar til å behandle et betydelig høyere antall forespørsler fra bakgrunnsapper.</span><span class="sxs-lookup"><span data-stu-id="e06fb-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="e06fb-109">**Overføre over 100 TB med data**</span><span class="sxs-lookup"><span data-stu-id="e06fb-109">**Migrating over 100TB of data**</span></span>

<span data-ttu-id="e06fb-110">Det ser ut til at du overfører over 100 TB med data til SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="e06fb-110">It appears you are migrating over 100TB of data to SharePoint Online.</span></span> <span data-ttu-id="e06fb-111">Vennligst følg trinnene nedenfor slik at vi kan hjelpe deg så snart som mulig.</span><span class="sxs-lookup"><span data-stu-id="e06fb-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="e06fb-112">Velg **Ny serviceforespørsel**, og deretter **Ny serviceforespørsel**.</span><span class="sxs-lookup"><span data-stu-id="e06fb-112">Select **New Service Request**, and then **New Service Request**.</span></span> 
2. <span data-ttu-id="e06fb-113">La tittelen og beskrivelsen være **SharePoint-overføring over 100 TB**.</span><span class="sxs-lookup"><span data-stu-id="e06fb-113">Leave the title and description as **SharePoint migration over 100TB**.</span></span>
3. <span data-ttu-id="e06fb-114">Når billetten er sendt inn, må du oppdatere den med følgende informasjon:</span><span class="sxs-lookup"><span data-stu-id="e06fb-114">Once the ticket has been submitted, please update it with the following information:</span></span> 

    - <span data-ttu-id="e06fb-115">Estimert størrelse på overføringen.</span><span class="sxs-lookup"><span data-stu-id="e06fb-115">Estimated size of your migration.</span></span>
    - <span data-ttu-id="e06fb-116">Et estimat på når du ønsker å starte og fullføre overføringen.</span><span class="sxs-lookup"><span data-stu-id="e06fb-116">An estimate of when you would like to start and complete your migration.</span></span>
    - <span data-ttu-id="e06fb-117">Beskriv hvor du overfører innholdet fra, for eksempel SharePoint Server, Box, GDrive, Fildelinger osv..</span><span class="sxs-lookup"><span data-stu-id="e06fb-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>


  

