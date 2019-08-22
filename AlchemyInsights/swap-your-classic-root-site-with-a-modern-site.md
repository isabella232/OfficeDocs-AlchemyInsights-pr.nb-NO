---
title: Bytt til klassisk rotområdet med et moderne område
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501088"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="cf11b-102">Bytt til klassisk rotområdet med et moderne område</span><span class="sxs-lookup"><span data-stu-id="cf11b-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="cf11b-103">Hvis miljøet er konfigurert før April 2019, kan du endre rotområdet til et moderne område ved hjelp av Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="cf11b-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="cf11b-104">Hvis du har et annet område som du vil bruke som rotområdet, kan du erstatte (swap) primært området med den.</span><span class="sxs-lookup"><span data-stu-id="cf11b-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="cf11b-105">Bruk [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen av et område med et annet område under arkivering av det opprinnelige området.</span><span class="sxs-lookup"><span data-stu-id="cf11b-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="cf11b-106">Tilgjengelig for både Team (ikke koblet til en gruppe) og kommunikasjon-området.</span><span class="sxs-lookup"><span data-stu-id="cf11b-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="cf11b-107">Flere muligheter blir introdusert snart som gjør at du kan fortsatt bruke innholdet på området, men du kan konvertere det eksisterende området til et område for kommunikasjon.</span><span class="sxs-lookup"><span data-stu-id="cf11b-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="cf11b-108">Disse funksjonene blir rullet gradvis.</span><span class="sxs-lookup"><span data-stu-id="cf11b-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="cf11b-109">Ta en titt på Office 365-Meldingssentral for oppdateringer.</span><span class="sxs-lookup"><span data-stu-id="cf11b-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="cf11b-110">Kjente problemer med bytte områder</span><span class="sxs-lookup"><span data-stu-id="cf11b-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="cf11b-111">Målområdet kan returnere en "not found" (HTTP 404)-feil for en kort tidsperiode.</span><span class="sxs-lookup"><span data-stu-id="cf11b-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="cf11b-112">Innhold må være kravlesøkt på nytt for å oppdatere søkeindeksen.</span><span class="sxs-lookup"><span data-stu-id="cf11b-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="cf11b-113">Det er ingen manuelle trinn nødvendig - dette vil bli gjort automatisk.</span><span class="sxs-lookup"><span data-stu-id="cf11b-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="cf11b-114">Alt avhengig av "statisk" koblinger (for eksempel filsynkronisering og OneNote-filer) må korrigeres manuelt.</span><span class="sxs-lookup"><span data-stu-id="cf11b-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="cf11b-115">Hvis kildeområdet var et område for nyheter i organisasjonen, kan du oppdatere URL-adressen.</span><span class="sxs-lookup"><span data-stu-id="cf11b-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="cf11b-116">Få en liste over alle organisasjonens nyhetsområder.</span><span class="sxs-lookup"><span data-stu-id="cf11b-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="cf11b-117">Project Server-områder må kanskje valideres for å sikre at de er fortsatt tilknyttet på riktig måte.</span><span class="sxs-lookup"><span data-stu-id="cf11b-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





