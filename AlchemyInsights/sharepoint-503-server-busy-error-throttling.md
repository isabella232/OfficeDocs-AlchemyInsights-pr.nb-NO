---
title: SharePoint Online regulere
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: c7881c0c7331e0aa74fcc439f52157bb75a56160
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559850"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="48a70-102">SharePoint Online regulere</span><span class="sxs-lookup"><span data-stu-id="48a70-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="48a70-103">Brukere kan få en 503-serveren er opptatt feil når du forsøker å gå til webområder for SharePoint- eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="48a70-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="48a70-104">Denne feilen kan være forårsaket av regulering i SharePoint-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="48a70-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="48a70-105">SharePoint Online bruker regulering til å opprettholde optimal ytelse og pålitelighet for SharePoint Online-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="48a70-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="48a70-106">Regulere begrenser kaller antall brukerhandlinger eller samtidige (som skript eller kode) for å hindre Overforbruk av ressurser.</span><span class="sxs-lookup"><span data-stu-id="48a70-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="48a70-107">Hvis du begrenset, 99% av tiden er det på grunn av egendefinert kode.</span><span class="sxs-lookup"><span data-stu-id="48a70-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="48a70-108">Hvis du vil ha mer informasjon om regulering, kan du se [unngå få begrenset eller blokkert i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="48a70-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="48a70-109">Hvis du tror denne feilen er relatert til regulering, kan du kontrollere om det finnes aktive vedlikehold oppstår på din leier ved å navigere til [Meldingssentral](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="48a70-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="48a70-110">Til slutt kontrollerer du besøker [Health Service](https://portal.office.com/adminportal/home#/servicehealth) -siden for å se etter veiledningene/hendelser som kan oppstå.</span><span class="sxs-lookup"><span data-stu-id="48a70-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

