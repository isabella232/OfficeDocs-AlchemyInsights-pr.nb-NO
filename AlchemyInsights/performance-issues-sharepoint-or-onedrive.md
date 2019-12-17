---
title: Ytelsesproblemer-SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068420"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="ecd3e-102">SharePoint eller OneDrive treg, utilgjengelig eller utilgjengelig for flere brukere</span><span class="sxs-lookup"><span data-stu-id="ecd3e-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="ecd3e-103">SharePoint eller OneDrive kan være treg, utilgjengelig eller utilgjengelig, eller kan vise tjenesten utilgjengelig eller 503 feil, av flere grunner:</span><span class="sxs-lookup"><span data-stu-id="ecd3e-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="ecd3e-104">Hvis SharePoint-eller OneDrive-området er tregt eller forsinket for flere brukere, kan det være et midlertidig tjeneste problem der brukere opplever uregelmessige forsinkelser eller navigasjonsfeil ved tilgang til SharePoint-områder eller OneDrive-innhold.</span><span class="sxs-lookup"><span data-stu-id="ecd3e-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="ecd3e-105">Kontroller [instrumentbordet for tjenestetilstand](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) for å se om organisasjonen er berørt.</span><span class="sxs-lookup"><span data-stu-id="ecd3e-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="ecd3e-106">Brukere kan få en *503-server er opptatt* feil når du prøver å navigere til SharePoint eller OneDrive-områder.</span><span class="sxs-lookup"><span data-stu-id="ecd3e-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="ecd3e-107">Denne feilen kan forårsakes av regulering i SharePoint-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="ecd3e-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="ecd3e-108">SharePoint Online bruker regulering for å opprettholde optimal ytelse og pålitelighet for SharePoint Online-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="ecd3e-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="ecd3e-109">Regulering begrenser antall brukerhandlinger eller samtidige anrop (etter skript eller kode) for å hindre overforbruk av ressurser.</span><span class="sxs-lookup"><span data-stu-id="ecd3e-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="ecd3e-110">Hvis du vil ha mer informasjon om regulering, kan du [unngå å få begrenset eller blokkert i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="ecd3e-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="ecd3e-111">Hvis du opplever treg ytelse med et **klassisk** eller **moderne** SharePoint-område eller-side, bruker du [side diagnoseverktøyet](https://aka.ms/perftool) til å analysere sidene.</span><span class="sxs-lookup"><span data-stu-id="ecd3e-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="ecd3e-112">Hvis du fremdeles opplever generell treg ytelse, kan du se gjennom ressursene nederst i denne artikkelen: [innføring i ytelsesjustering for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="ecd3e-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  