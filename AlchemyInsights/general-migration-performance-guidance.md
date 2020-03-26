---
title: Generell veiledning for ytelsesoverføring
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932487"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="dae58-102">Generell veiledning for ytelsesoverføring</span><span class="sxs-lookup"><span data-stu-id="dae58-102">General migration performance guidance</span></span>

<span data-ttu-id="dae58-103">**Viktig**: mange SharePoint Online- og OneDrive-kunder kjører bedriftskritiske programmer mot tjenesten som kjører i bakgrunnen.</span><span class="sxs-lookup"><span data-stu-id="dae58-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="dae58-104">Disse omfatter innholdsoverføring, hindring av tap av data (DLP) og sikkerhetskopiløsninger.</span><span class="sxs-lookup"><span data-stu-id="dae58-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="dae58-105">I denne uforutsigbare tiden vi nå lever i er det viktigere enn noensinne at tjenestene våre er pålitelige, derfor utfører vi flere tiltakstrinn for å sikre at SharePoint Online-og OneDrive-tjenestene forblir svært tilgjengelig for de brukerne som er avhengige av tjenesten for å utføre et eksternt arbeid.</span><span class="sxs-lookup"><span data-stu-id="dae58-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="dae58-106">For å støtte dette målet har vi implementert strengere begrensninger for bakgrunnsappene (overføring, DLP og sikkerhetskopieringsløsninger) i løpet av hverdager på dagtid.</span><span class="sxs-lookup"><span data-stu-id="dae58-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="dae58-107">Du bør derfor forvente at disse appene har svært begrenset kapasitet på disse tidspunktene.</span><span class="sxs-lookup"><span data-stu-id="dae58-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="dae58-108">Men på kvelden og i helgene står tjenesten klar til å behandle et betydelig høyere antall forespørsler fra regionenes bakgrunnsapper.</span><span class="sxs-lookup"><span data-stu-id="dae58-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="dae58-109">**Veiledning for overføringsytelse**</span><span class="sxs-lookup"><span data-stu-id="dae58-109">**Migration performance guidance**</span></span>

<span data-ttu-id="dae58-110">Overføringsytelsen kan påvirkes av nettverkets infrastruktur, filstørrelse, overføringstid og begrensning.</span><span class="sxs-lookup"><span data-stu-id="dae58-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="dae58-111">Hvis du har en forståelse av disse, vil det hjelpe deg med å planlegge og maksimere effektiviteten av overføringen din.</span><span class="sxs-lookup"><span data-stu-id="dae58-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="dae58-112">Generell veiledning for ytelsesoverføring</span><span class="sxs-lookup"><span data-stu-id="dae58-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
