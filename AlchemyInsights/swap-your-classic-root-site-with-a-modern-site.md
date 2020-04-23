---
title: Bytt ditt klassiske rotnettsted med et moderne nettsted
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741553"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="d40ae-102">Bytt ditt klassiske rotnettsted med et moderne nettsted</span><span class="sxs-lookup"><span data-stu-id="d40ae-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="d40ae-103">Hvis miljøet ble konfigurert før april 2019, kan du endre rotområdet til et moderne område ved hjelp av Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="d40ae-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="d40ae-104">Hvis du har et annet nettsted som du vil bruke som rotområde, kan du erstatte [(bytte) rotområdet](https://docs.microsoft.com/sharepoint/modern-root-site) med det.</span><span class="sxs-lookup"><span data-stu-id="d40ae-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="d40ae-105">Bruk [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen av et område med et annet område mens du arkiverer det opprinnelige området.</span><span class="sxs-lookup"><span data-stu-id="d40ae-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="d40ae-106">Tilgjengelig for både gruppeområde (ikke koblet til en gruppe) og kommunikasjonsområde.</span><span class="sxs-lookup"><span data-stu-id="d40ae-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="d40ae-107">Ytterligere funksjoner vil bli introdusert snart som vil tillate deg å fortsette å bruke innholdet på nettstedet, men konvertere det eksisterende området til et kommunikasjonsområde.</span><span class="sxs-lookup"><span data-stu-id="d40ae-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="d40ae-108">Disse egenskapene vil bli rullet ut gradvis.</span><span class="sxs-lookup"><span data-stu-id="d40ae-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="d40ae-109">Fortsett å se etter oppdateringer i meldingssenteret.</span><span class="sxs-lookup"><span data-stu-id="d40ae-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="d40ae-110">Kjente problemer med bytte nettsteder</span><span class="sxs-lookup"><span data-stu-id="d40ae-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="d40ae-111">Målområdet kan returnere en "ikke funnet" (HTTP 404) feil i en kort periode.</span><span class="sxs-lookup"><span data-stu-id="d40ae-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="d40ae-112">Innholdet må søkes på nytt for å oppdatere søkeindeksen.</span><span class="sxs-lookup"><span data-stu-id="d40ae-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="d40ae-113">Det er ikke nødvendig med manuelt trinn - dette vil bli gjort automatisk.</span><span class="sxs-lookup"><span data-stu-id="d40ae-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="d40ae-114">Alt som er avhengig av "statiske" koblinger (for eksempel Filsynkronisering og OneNote-filer), må korrigeres manuelt.</span><span class="sxs-lookup"><span data-stu-id="d40ae-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="d40ae-115">Hvis kildeområdet var et organisasjonsnyhetsnettsted, oppdaterer du URL-adressen.</span><span class="sxs-lookup"><span data-stu-id="d40ae-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="d40ae-116">Få en liste over alle organisatoriske nyhetssider.</span><span class="sxs-lookup"><span data-stu-id="d40ae-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="d40ae-117">Project Server-områder må kanskje valideres for å sikre at de fortsatt er tilknyttet på riktig måte.</span><span class="sxs-lookup"><span data-stu-id="d40ae-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
