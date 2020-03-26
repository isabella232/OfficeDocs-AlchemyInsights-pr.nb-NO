---
title: Overføre til SharePoint Online via Overføringsveiviseren
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
- "3192"
ms.openlocfilehash: 5aebf7903670e74f616c8f151749d760caf1d642
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932187"
---
# <a name="migrating-to-sharepoint-online-via-migration-manager"></a><span data-ttu-id="24385-102">Overføre til SharePoint Online via Overføringsveiviseren</span><span class="sxs-lookup"><span data-stu-id="24385-102">Migrating to SharePoint Online via Migration Manager</span></span>

<span data-ttu-id="24385-103">**Viktig**: mange SharePoint Online- og OneDrive-kunder kjører bedriftskritiske programmer mot tjenesten som kjører i bakgrunnen.</span><span class="sxs-lookup"><span data-stu-id="24385-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="24385-104">Disse omfatter innholdsoverføring, hindring av tap av data (DLP) og sikkerhetskopiløsninger.</span><span class="sxs-lookup"><span data-stu-id="24385-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="24385-105">I denne uforutsigbare tiden vi nå lever i er det viktigere enn noensinne at tjenestene våre er pålitelige, derfor utfører vi flere tiltakstrinn for å sikre at SharePoint Online-og OneDrive-tjenestene forblir svært tilgjengelig for de brukerne som er avhengige av tjenesten for å utføre et eksternt arbeid.</span><span class="sxs-lookup"><span data-stu-id="24385-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="24385-106">For å støtte dette målet har vi implementert strengere begrensninger for bakgrunnsappene (overføring, DLP og sikkerhetskopieringsløsninger) i løpet av hverdager på dagtid.</span><span class="sxs-lookup"><span data-stu-id="24385-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="24385-107">Du bør derfor forvente at disse appene har svært begrenset kapasitet på disse tidspunktene.</span><span class="sxs-lookup"><span data-stu-id="24385-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="24385-108">Men på kvelden og i helgene står tjenesten klar til å behandle et betydelig høyere antall forespørsler fra regionenes bakgrunnsapper.</span><span class="sxs-lookup"><span data-stu-id="24385-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="24385-109">**Overføringsveiviseren**</span><span class="sxs-lookup"><span data-stu-id="24385-109">**Migration Manager**</span></span>

<span data-ttu-id="24385-110">Overføringsveiviseren finner du i det moderne SharePoint-administrasjonssenteret, som veileder deg gjennom konfigurasjonen av klientene og opprettelsen av oppgavene dine.</span><span class="sxs-lookup"><span data-stu-id="24385-110">Located in the modern SharePoint Admin Center, the Migration Manager guides you through the setup of your clients and the creation of your tasks.</span></span> <span data-ttu-id="24385-111">Du kan angi globale innstillinger eller innstillinger for aktivitetsnivå, se hele oppgavens fremdrift og laste ned aggregerte sammendrags- og oppgavenivårapporter.</span><span class="sxs-lookup"><span data-stu-id="24385-111">You can specify global or task-level settings, view all-up task progress, and download aggregated summary and task-level reports.</span></span>

- [<span data-ttu-id="24385-112">Kom i gang med overføringsveiviseren</span><span class="sxs-lookup"><span data-stu-id="24385-112">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="24385-113">Konfigurer overføringsveiviserens klienter</span><span class="sxs-lookup"><span data-stu-id="24385-113">Setup Migration Manager clients</span></span>](https://docs.microsoft.com/sharepointmigration/mm-setup-clients)

- [<span data-ttu-id="24385-114">Innstillinger for overføringsveiviseren</span><span class="sxs-lookup"><span data-stu-id="24385-114">Migration Manager Settings</span></span>](https://docs.microsoft.com/sharepointmigration/mm-settings)
