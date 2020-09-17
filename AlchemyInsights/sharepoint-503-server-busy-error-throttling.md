---
title: Begrensning av SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773856"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="5b59e-102">Begrensning av SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5b59e-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="5b59e-103">**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="5b59e-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="5b59e-104">**503 server er opptatt-feil**</span><span class="sxs-lookup"><span data-stu-id="5b59e-104">**503 server is busy error**</span></span>

<span data-ttu-id="5b59e-105">Brukere kan få en 503-server er opptatt-feil ved forsøk på å navigere til SharePoint-eller OneDrive-nettsteder.</span><span class="sxs-lookup"><span data-stu-id="5b59e-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="5b59e-106">Denne feilen kan være forårsaket av begrensning i SharePoint-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="5b59e-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="5b59e-107">SharePoint Online bruker begrensning til å opprettholde optimal ytelse og pålitelighet for SharePoint Online-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="5b59e-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="5b59e-108">Begrensning begrenser antall brukerhandlinger eller samtidige anrop (via skript eller kode) for å hindre overforbruk av ressurser.</span><span class="sxs-lookup"><span data-stu-id="5b59e-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="5b59e-109">Hvis du vil ha mer informasjon om begrensning, kan du [unngå å bli begrenset eller blokkert i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="5b59e-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="5b59e-110">Hvis du tror denne feilen er ikke relatert til begrensning, kan du kontrollere om det er aktivt vedlikehold som oppstår på leieren, ved å navigere til [meldings senteret](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="5b59e-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="5b59e-111">Til slutt må du gå til siden for [tjeneste tilstand](https://portal.office.com/adminportal/home#/servicehealth) for å kontrollere eventuelle rådgivere/hendelser som kan oppstå.</span><span class="sxs-lookup"><span data-stu-id="5b59e-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

