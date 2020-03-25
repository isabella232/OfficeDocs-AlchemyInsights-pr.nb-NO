---
title: SharePoint-overføring med SPMT
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2594"
ms.openlocfilehash: e7719d1fc6dda0d5bd340775219401dade2933fe
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931559"
---
# <a name="sharepoint-migration-with-spmt"></a><span data-ttu-id="1329f-102">SharePoint-overføring med SPMT</span><span class="sxs-lookup"><span data-stu-id="1329f-102">SharePoint Migration with SPMT</span></span>

<span data-ttu-id="1329f-103">**Viktig:** Mange SharePoint Online- og OneDrive-kunder kjører forretningskritiske programmer mot tjenesten som kjører i bakgrunnen.</span><span class="sxs-lookup"><span data-stu-id="1329f-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="1329f-104">Disse inkluderer innholdsoverføring, Hindring av tap av data (DLP) og sikkerhetskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="1329f-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="1329f-105">I løpet av disse enestående tider tar vi skritt for å sikre at SharePoint Online- og OneDrive-tjenester forblir svært tilgjengelige og pålitelige for brukerne som er avhengige av tjenesten mer enn noensinne i scenarier for eksternt arbeid.</span><span class="sxs-lookup"><span data-stu-id="1329f-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="1329f-106">Til støtte for dette målet har vi implementert strammere reguleringsgrenser for bakgrunnsapper (overførings-, DLP- og sikkerhetskopieringsløsninger) i løpet av ukedagsdagstimene.</span><span class="sxs-lookup"><span data-stu-id="1329f-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="1329f-107">Du bør forvente at disse appene vil oppnå svært begrenset gjennomstrømning i disse tider.</span><span class="sxs-lookup"><span data-stu-id="1329f-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="1329f-108">I løpet av kvelds- og helgetiden for regionen vil tjenesten imidlertid være klar til å behandle et betydelig høyere antall forespørsler fra bakgrunnsapper.</span><span class="sxs-lookup"><span data-stu-id="1329f-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="1329f-109">**Overføringsverktøyet for SharePoint**</span><span class="sxs-lookup"><span data-stu-id="1329f-109">**SharePoint Migration Tool**</span></span>

<span data-ttu-id="1329f-110">SharePoint Migration Tool er utformet for å brukes til overføringer som spenner fra det minste settet med filer til en storskala enterprise-overføring, og vil tillate deg å overføre informasjonen til skyen og dra nytte av det nyeste samarbeidet, intelligensen og sikkerhetsløsninger med Office 365.</span><span class="sxs-lookup"><span data-stu-id="1329f-110">Designed to be used for migrations ranging from the smallest set of files to a large scale enterprise migration, the SharePoint Migration Tool will allow you to transfer your information to the cloud and take advantage of the newest collaboration, intelligence, and security solutions with Office 365.</span></span>

- [<span data-ttu-id="1329f-111">Laste ned og installere SharePoint Migration Tool</span><span class="sxs-lookup"><span data-stu-id="1329f-111">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
- [<span data-ttu-id="1329f-112">Feilsøke vanlige SPMT-problemer og feil</span><span class="sxs-lookup"><span data-stu-id="1329f-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
- [<span data-ttu-id="1329f-113">Feilsøke problemer med SPMT-installasjonen</span><span class="sxs-lookup"><span data-stu-id="1329f-113">Troubleshooting SPMT installation issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues#troubleshooting-spmt-installation-issues)
