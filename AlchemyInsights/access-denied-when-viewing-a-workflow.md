---
title: Ingen tilgang når du viser en arbeidsflyt
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/25/2019
ms.locfileid: "36747757"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="fe3ed-102">Ingen tilgang når du viser en arbeidsflyt</span><span class="sxs-lookup"><span data-stu-id="fe3ed-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="fe3ed-103">SharePoint 2013 arbeidsflyter som prøver å sende en e-post til en SharePoint-gruppe kan mislykkes med feilmeldingen "ingen tilgang" Hvis medlemskapet i SharePoint-gruppen ikke er satt til alle.</span><span class="sxs-lookup"><span data-stu-id="fe3ed-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="fe3ed-104">**Hvis du vil løse dette problemet, gjør du følgende:**</span><span class="sxs-lookup"><span data-stu-id="fe3ed-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="fe3ed-105">Tillat alle å se medlemmene av SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="fe3ed-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="fe3ed-106">Fjern SharePoint-gruppen fra til-eller kopi-linjen i e-postmeldingen.</span><span class="sxs-lookup"><span data-stu-id="fe3ed-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="fe3ed-107">Legg til brukerne eksplisitt i til-eller kopi-linjen hvis medlemskaps synligheten ikke kan endres for SharePoint-gruppe.</span><span class="sxs-lookup"><span data-stu-id="fe3ed-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="fe3ed-108">For å se flere detaljer henvises det til [http uautorisert til/_vti_bin/Client.SVC/Sp.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="fe3ed-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  