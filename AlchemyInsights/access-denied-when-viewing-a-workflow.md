---
title: Ingen tilgang når du viser en arbeidsflyt
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 53bd9285e49e220f880eea21923f261302003127
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495832"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="b8448-102">Ingen tilgang når du viser en arbeidsflyt</span><span class="sxs-lookup"><span data-stu-id="b8448-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="b8448-103">SharePoint 2013 arbeidsflyter som forsøker å sende en e-post til en SharePoint-gruppe kan mislykkes med en feilmelding av typen "Ingen tilgang" Hvis medlemskap for SharePoint-gruppen ikke er satt til alle.</span><span class="sxs-lookup"><span data-stu-id="b8448-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="b8448-104">**Hvis du vil løse dette problemet, gjør du følgende:**</span><span class="sxs-lookup"><span data-stu-id="b8448-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="b8448-105">Tillat alle å se medlemmer av SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="b8448-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="b8448-106">Fjern SharePoint-gruppen fra til- eller Kopi-linjen i e-postmeldingen.</span><span class="sxs-lookup"><span data-stu-id="b8448-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="b8448-107">Legge til brukere eksplisitt i til- eller kopi linje hvis medlemskap synligheten ikke kan endres for SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="b8448-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="b8448-108">Hvis du vil vise flere detaljer kan du se [HTTP uautorisert til /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="b8448-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  