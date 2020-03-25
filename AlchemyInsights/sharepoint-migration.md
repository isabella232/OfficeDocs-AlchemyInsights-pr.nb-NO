---
title: Overføre alternativer til SharePoint Online
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932739"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="ddb46-102">Overføre alternativer til SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="ddb46-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="ddb46-103">**Viktig:** Mange SharePoint Online- og OneDrive-kunder kjører forretningskritiske programmer mot tjenesten som kjører i bakgrunnen.</span><span class="sxs-lookup"><span data-stu-id="ddb46-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="ddb46-104">Disse inkluderer innholdsoverføring, Hindring av tap av data (DLP) og sikkerhetskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="ddb46-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="ddb46-105">I løpet av disse enestående tider tar vi skritt for å sikre at SharePoint Online- og OneDrive-tjenester forblir svært tilgjengelige og pålitelige for brukerne som er avhengige av tjenesten mer enn noensinne i scenarier for eksternt arbeid.</span><span class="sxs-lookup"><span data-stu-id="ddb46-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="ddb46-106">Til støtte for dette målet har vi implementert strammere reguleringsgrenser for bakgrunnsapper (overførings-, DLP- og sikkerhetskopieringsløsninger) i løpet av ukedagsdagstimene.</span><span class="sxs-lookup"><span data-stu-id="ddb46-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="ddb46-107">Du bør forvente at disse appene vil oppnå svært begrenset gjennomstrømning i disse tider.</span><span class="sxs-lookup"><span data-stu-id="ddb46-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="ddb46-108">I løpet av kvelds- og helgetiden for regionen vil tjenesten imidlertid være klar til å behandle et betydelig høyere antall forespørsler fra bakgrunnsapper.</span><span class="sxs-lookup"><span data-stu-id="ddb46-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="ddb46-109">**Alternativer for overføring**</span><span class="sxs-lookup"><span data-stu-id="ddb46-109">**Migration options**</span></span>

<span data-ttu-id="ddb46-110">Det finnes forskjellige alternativer som er tilgjengelige for å overføre innhold til SharePoint Online, avhengig av størrelsen og antallet filer du må flytte, kan du se en liste over alternativer [som finnes her](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="ddb46-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="ddb46-111">Hvis du vil ha mer informasjon om innholdsoverføring, kan du gå til koblingene nedenfor.</span><span class="sxs-lookup"><span data-stu-id="ddb46-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="ddb46-112">Verktøy for overføring av SharePoint</span><span class="sxs-lookup"><span data-stu-id="ddb46-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="ddb46-113">Kom i gang med overføringsbehandling</span><span class="sxs-lookup"><span data-stu-id="ddb46-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="ddb46-114">Overføringshastighet for Sharepoint Online og ODB</span><span class="sxs-lookup"><span data-stu-id="ddb46-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="ddb46-115">Unngå å bli strupet eller blokkert i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="ddb46-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="ddb46-116">SharePoint Migration Assessment Tool (SMAT)</span><span class="sxs-lookup"><span data-stu-id="ddb46-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="ddb46-117">**Merk:** For øyeblikket støtter SharePoint-overføringsverktøyet bare overføringer fra SharePoint 2010 og 2013.</span><span class="sxs-lookup"><span data-stu-id="ddb46-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="ddb46-118">Versjon 2016 eller 2019 støttes ikke for øyeblikket.</span><span class="sxs-lookup"><span data-stu-id="ddb46-118">Version 2016 or 2019 are not supported at this time.</span></span>
