---
title: Ingen tilgang når du viser en arbeids flyt
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688811"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="e62b5-102">Ingen tilgang når du viser en arbeids flyt</span><span class="sxs-lookup"><span data-stu-id="e62b5-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="e62b5-103">SharePoint 2013-arbeids flyter som prøver å sende en e-postmelding til en SharePoint-gruppe, kan mislykkes med feil meldingen «ingen tilgang» hvis medlemskapet i SharePoint-gruppen ikke er satt til alle.</span><span class="sxs-lookup"><span data-stu-id="e62b5-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="e62b5-104">**Du kan løse dette problemet ved å gjøre følgende:**</span><span class="sxs-lookup"><span data-stu-id="e62b5-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="e62b5-105">La alle se medlemmene i SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="e62b5-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="e62b5-106">Fjern SharePoint-gruppen fra til-eller kopi-linjen i e-postmeldingen.</span><span class="sxs-lookup"><span data-stu-id="e62b5-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="e62b5-107">Legg til brukerne eksplisitt i til-eller kopi linjen hvis medlemskaps synligheten ikke kan endres for SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="e62b5-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="e62b5-108">Hvis du vil vise flere detaljer, kan du se [http uautorisert til/_vti_bin/Client.SVC/Sp.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="e62b5-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  