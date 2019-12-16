---
title: Ingen tilgang når du viser en arbeidsflyt
ms.author: pebaum
author: pebaum
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 1cfda8e08ada05858a28f2bede8c31261f9de351
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050534"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="9b523-102">Ingen tilgang når du viser en arbeidsflyt</span><span class="sxs-lookup"><span data-stu-id="9b523-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="9b523-103">SharePoint 2013 arbeidsflyter som prøver å sende en e-post til en SharePoint-gruppe kan mislykkes med feilmeldingen "ingen tilgang" Hvis medlemskapet i SharePoint-gruppen ikke er satt til alle.</span><span class="sxs-lookup"><span data-stu-id="9b523-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="9b523-104">**Hvis du vil løse dette problemet, gjør du følgende:**</span><span class="sxs-lookup"><span data-stu-id="9b523-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="9b523-105">Tillat alle å se medlemmene av SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="9b523-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="9b523-106">Fjern SharePoint-gruppen fra til-eller kopi-linjen i e-postmeldingen.</span><span class="sxs-lookup"><span data-stu-id="9b523-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="9b523-107">Legg til brukerne eksplisitt i til-eller kopi-linjen hvis medlemskaps synligheten ikke kan endres for SharePoint-gruppe.</span><span class="sxs-lookup"><span data-stu-id="9b523-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="9b523-108">For å se flere detaljer henvises det til [http uautorisert til/_vti_bin/Client.SVC/Sp.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="9b523-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  