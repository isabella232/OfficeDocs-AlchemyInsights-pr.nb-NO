---
title: SharePoint Online regulering
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931235"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="f0567-102">SharePoint Online regulering</span><span class="sxs-lookup"><span data-stu-id="f0567-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="f0567-103">**Viktig:** Mange SharePoint Online- og OneDrive-kunder kjører forretningskritiske programmer mot tjenesten som kjører i bakgrunnen.</span><span class="sxs-lookup"><span data-stu-id="f0567-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f0567-104">Disse inkluderer innholdsoverføring, Hindring av tap av data (DLP) og sikkerhetskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="f0567-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f0567-105">I løpet av disse enestående tider tar vi skritt for å sikre at SharePoint Online- og OneDrive-tjenester forblir svært tilgjengelige og pålitelige for brukerne som er avhengige av tjenesten mer enn noensinne i scenarier for eksternt arbeid.</span><span class="sxs-lookup"><span data-stu-id="f0567-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f0567-106">Til støtte for dette målet har vi implementert strammere reguleringsgrenser for bakgrunnsapper (overførings-, DLP- og sikkerhetskopieringsløsninger) i løpet av ukedagsdagstimene.</span><span class="sxs-lookup"><span data-stu-id="f0567-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f0567-107">Du bør forvente at disse appene vil oppnå svært begrenset gjennomstrømning i disse tider.</span><span class="sxs-lookup"><span data-stu-id="f0567-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f0567-108">I løpet av kvelds- og helgetiden for regionen vil tjenesten imidlertid være klar til å behandle et betydelig høyere antall forespørsler fra bakgrunnsapper.</span><span class="sxs-lookup"><span data-stu-id="f0567-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f0567-109">**503-serveren er opptatt feil**</span><span class="sxs-lookup"><span data-stu-id="f0567-109">**503 server is busy error**</span></span>

<span data-ttu-id="f0567-110">Brukere kan få en 503-server er opptatt feil når du prøver å navigere til SharePoint eller OneDrive-områder.</span><span class="sxs-lookup"><span data-stu-id="f0567-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="f0567-111">Denne feilen kan skyldes regulering i SharePoint-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="f0567-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="f0567-112">SharePoint Online bruker regulering for å opprettholde optimal ytelse og pålitelighet for SharePoint Online-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="f0567-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="f0567-113">Regulering begrenser antall brukerhandlinger eller samtidige anrop (etter skript eller kode) for å forhindre overforbruk av ressurser.</span><span class="sxs-lookup"><span data-stu-id="f0567-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="f0567-114">Hvis du vil ha mer informasjon om regulering, [se, Unngå å bli strupet eller blokkert i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="f0567-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="f0567-115">Hvis du mener at denne feilen ikke er relatert til regulering, kan du kontrollere om det oppstår aktivt vedlikehold på leieren ved å navigere til [meldingssenteret](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="f0567-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="f0567-116">Til slutt må du sørge for at du besøker [Siden Servicehelse](https://portal.office.com/adminportal/home#/servicehealth) for å se etter eventuelle råd/hendelser som kan forekomme.</span><span class="sxs-lookup"><span data-stu-id="f0567-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

