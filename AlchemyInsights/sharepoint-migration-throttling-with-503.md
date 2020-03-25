---
title: SharePoint-overføring struping med 503 feil
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931667"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="d8016-102">SharePoint-overføring struping med 503 feil</span><span class="sxs-lookup"><span data-stu-id="d8016-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="d8016-103">**Viktig:** Mange SharePoint Online- og OneDrive-kunder kjører forretningskritiske programmer mot tjenesten som kjører i bakgrunnen.</span><span class="sxs-lookup"><span data-stu-id="d8016-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="d8016-104">Disse inkluderer innholdsoverføring, Hindring av tap av data (DLP) og sikkerhetskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="d8016-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="d8016-105">I løpet av disse enestående tider tar vi skritt for å sikre at SharePoint Online- og OneDrive-tjenester forblir svært tilgjengelige og pålitelige for brukerne som er avhengige av tjenesten mer enn noensinne i scenarier for eksternt arbeid.</span><span class="sxs-lookup"><span data-stu-id="d8016-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="d8016-106">Til støtte for dette målet har vi implementert strammere reguleringsgrenser for bakgrunnsapper (overførings-, DLP- og sikkerhetskopieringsløsninger) i løpet av ukedagsdagstimene.</span><span class="sxs-lookup"><span data-stu-id="d8016-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="d8016-107">Du bør forvente at disse appene vil oppnå svært begrenset gjennomstrømning i disse tider.</span><span class="sxs-lookup"><span data-stu-id="d8016-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="d8016-108">I løpet av kvelds- og helgetiden for regionen vil tjenesten imidlertid være klar til å behandle et betydelig høyere antall forespørsler fra bakgrunnsapper.</span><span class="sxs-lookup"><span data-stu-id="d8016-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="d8016-109">**503 feil når du overfører til SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="d8016-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="d8016-110">Det ser ut til at du overfører til SharePoint Online og mottar 503 feil.</span><span class="sxs-lookup"><span data-stu-id="d8016-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="d8016-111">Vennligst følg trinnene nedenfor slik at vi kan hjelpe deg så snart som mulig.</span><span class="sxs-lookup"><span data-stu-id="d8016-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="d8016-112">Klikk **Kontaktkundestøtte**, og deretter **Ny serviceforespørsel**.</span><span class="sxs-lookup"><span data-stu-id="d8016-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="d8016-113">For tittelen og beskrivelsen skriver du inn **SharePoint Migration Throttling med 503**.</span><span class="sxs-lookup"><span data-stu-id="d8016-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="d8016-114">Når billetten er sendt inn, må du oppdatere den med følgende informasjon:</span><span class="sxs-lookup"><span data-stu-id="d8016-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="d8016-115">Hvor mye igjen av migrering (for eksempel hvor mange TBer?).</span><span class="sxs-lookup"><span data-stu-id="d8016-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="d8016-116">Start- og sluttdatoen for overføring.</span><span class="sxs-lookup"><span data-stu-id="d8016-116">Migration start and end date.</span></span>
    - <span data-ttu-id="d8016-117">Beskriv hvor du overfører innholdet fra, for eksempel SharePoint Server, Box, GDrive, Fildelinger osv..</span><span class="sxs-lookup"><span data-stu-id="d8016-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="d8016-118">Estimer antall gassfall (for eksempel x gass per time?) og når skjedde strupingen.</span><span class="sxs-lookup"><span data-stu-id="d8016-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="d8016-119">Hvilket overføringsverktøy du bruker (for eksempel SPMT eller ShareGate).</span><span class="sxs-lookup"><span data-stu-id="d8016-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


