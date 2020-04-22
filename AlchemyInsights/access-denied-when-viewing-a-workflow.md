---
title: Ingen tilgang når du viser en arbeidsflyt
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687339"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="76d47-102">Ingen tilgang når du viser en arbeidsflyt</span><span class="sxs-lookup"><span data-stu-id="76d47-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="76d47-103">SharePoint 2013 arbeidsflyter som prøver å sende en e-post til en SharePoint-gruppe, kan mislykkes med feilmeldingen "Ingen tilgang" hvis medlemskapet i SharePoint-gruppen ikke er satt til Alle.</span><span class="sxs-lookup"><span data-stu-id="76d47-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="76d47-104">**Hvis du vil løse dette problemet, gjør du følgende:**</span><span class="sxs-lookup"><span data-stu-id="76d47-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="76d47-105">La alle se medlemmene av SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="76d47-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="76d47-106">Fjern SharePoint-gruppen fra Til- eller KOPI-linjen i e-posten.</span><span class="sxs-lookup"><span data-stu-id="76d47-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="76d47-107">Legg eksplisitt til brukerne på til- eller KOPI-linjen hvis ansvarssynligheten ikke kan endres for SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="76d47-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="76d47-108">Hvis du vil vise flere detaljer, kan du se [HTTP uautorisert til /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="76d47-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  