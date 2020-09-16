---
title: Ytelses problemer – SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771910"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="5a56c-102">SharePoint eller OneDrive langsomt, utilgjengelig eller ikke tilgjengelig for flere brukere</span><span class="sxs-lookup"><span data-stu-id="5a56c-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="5a56c-103">SharePoint eller OneDrive kan være tregt, ikke tilgjengelig eller utilgjengelig, eller kan vise tjeneste utilgjengelig eller 503 feil, av flere årsaker:</span><span class="sxs-lookup"><span data-stu-id="5a56c-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="5a56c-104">Hvis SharePoint-eller OneDrive-nettstedet er tregt eller forsinket for flere brukere, kan det oppstå et midlertidig tjeneste problem der brukere opplever periodiske forsinkelser eller navigasjons feil ved tilgang til SharePoint-nettsteder eller OneDrive-innhold.</span><span class="sxs-lookup"><span data-stu-id="5a56c-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="5a56c-105">Kontroller [instrument bordet for tjeneste tilstand](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) for å se om organisasjonen er berørt.</span><span class="sxs-lookup"><span data-stu-id="5a56c-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="5a56c-106">Brukere kan få en *503-server er opptatt-* feil ved forsøk på å navigere til SharePoint-eller OneDrive-nettsteder.</span><span class="sxs-lookup"><span data-stu-id="5a56c-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="5a56c-107">Denne feilen kan være forårsaket av begrensning i SharePoint-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="5a56c-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="5a56c-108">SharePoint Online bruker begrensning til å opprettholde optimal ytelse og pålitelighet for SharePoint Online-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="5a56c-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="5a56c-109">Begrensning begrenser antall brukerhandlinger eller samtidige anrop (via skript eller kode) for å hindre overforbruk av ressurser.</span><span class="sxs-lookup"><span data-stu-id="5a56c-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="5a56c-110">Hvis du vil ha mer informasjon om begrensning, kan du [unngå å bli begrenset eller blokkert i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="5a56c-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="5a56c-111">Hvis du opplever lav ytelse med et **klassisk** eller **moderne** SharePoint-nettsted eller-side, bruker du [side diagnose verktøyet](https://aka.ms/perftool) til å analysere sidene.</span><span class="sxs-lookup"><span data-stu-id="5a56c-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="5a56c-112">Hvis du fremdeles opplever generell dårlig ytelse, kan du se gjennom ressursene nederst i denne artikkelen: [innføring i ytelses justering for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="5a56c-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  