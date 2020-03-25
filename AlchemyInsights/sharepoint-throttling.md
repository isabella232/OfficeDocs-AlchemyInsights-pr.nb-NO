---
title: SharePoint Online-regulering
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931451"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="79d0b-102">SharePoint Online-regulering</span><span class="sxs-lookup"><span data-stu-id="79d0b-102">SharePoint Online throttling</span></span>

<span data-ttu-id="79d0b-103">**Viktig:** Mange SharePoint Online- og OneDrive-kunder kjører forretningskritiske programmer mot tjenesten som kjører i bakgrunnen.</span><span class="sxs-lookup"><span data-stu-id="79d0b-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="79d0b-104">Disse inkluderer innholdsoverføring, Hindring av tap av data (DLP) og sikkerhetskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="79d0b-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="79d0b-105">I løpet av disse enestående tider tar vi skritt for å sikre at SharePoint Online- og OneDrive-tjenester forblir svært tilgjengelige og pålitelige for brukerne som er avhengige av tjenesten mer enn noensinne i scenarier for eksternt arbeid.</span><span class="sxs-lookup"><span data-stu-id="79d0b-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="79d0b-106">Til støtte for dette målet har vi implementert strammere reguleringsgrenser for bakgrunnsapper (overførings-, DLP- og sikkerhetskopieringsløsninger) i løpet av ukedagsdagstimene.</span><span class="sxs-lookup"><span data-stu-id="79d0b-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="79d0b-107">Du bør forvente at disse appene vil oppnå svært begrenset gjennomstrømning i disse tider.</span><span class="sxs-lookup"><span data-stu-id="79d0b-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="79d0b-108">I løpet av kvelds- og helgetiden for regionen vil tjenesten imidlertid være klar til å behandle et betydelig høyere antall forespørsler fra bakgrunnsapper.</span><span class="sxs-lookup"><span data-stu-id="79d0b-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="79d0b-109">**SharePoint Online-regulering**</span><span class="sxs-lookup"><span data-stu-id="79d0b-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="79d0b-110">SharePoint Online bruker regulering for å opprettholde optimal ytelse og pålitelighet for SharePoint Online-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="79d0b-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="79d0b-111">Regulering begrenser antall brukerhandlinger eller samtidige anrop (etter skript eller kode) for å forhindre overforbruk av ressurser.</span><span class="sxs-lookup"><span data-stu-id="79d0b-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="79d0b-112">For mer informasjon, vennligst besøk linkene nedenfor.</span><span class="sxs-lookup"><span data-stu-id="79d0b-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="79d0b-113">Unngå å bli strupet eller blokkert i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="79d0b-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="79d0b-114">Dataoverføring og SPO-regulering</span><span class="sxs-lookup"><span data-stu-id="79d0b-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="79d0b-115">Overføringshastighet for SharePoint Online og OneDrive</span><span class="sxs-lookup"><span data-stu-id="79d0b-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="79d0b-116">Håndtere SharePoint Online-regulering ved hjelp av eksponentiell tilbake</span><span class="sxs-lookup"><span data-stu-id="79d0b-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="79d0b-117">Kapasitetsplanlegging og lasttesting SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="79d0b-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

