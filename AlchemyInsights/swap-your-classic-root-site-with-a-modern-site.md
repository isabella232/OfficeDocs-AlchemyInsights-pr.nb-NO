---
title: Bytt ut ditt klassiske rotområde med et moderne nettsted
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: fe1f0f662c49de2bd0b5b997697c98309cb7983f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042936"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="79050-102">Bytt ut ditt klassiske rotområde med et moderne nettsted</span><span class="sxs-lookup"><span data-stu-id="79050-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="79050-103">Hvis miljøet ble konfigurert før april 2019, kan du endre det primære området til et moderne område ved hjelp av Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="79050-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="79050-104">Hvis du har et annet område som du vil bruke som ditt primære webområde, kan du erstatte [(bytte) det primære området](https://docs.microsoft.com/sharepoint/modern-root-site) med det.</span><span class="sxs-lookup"><span data-stu-id="79050-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="79050-105">Bruk [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen av et område med et annet område under arkivering av det opprinnelige området.</span><span class="sxs-lookup"><span data-stu-id="79050-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="79050-106">Tilgjengelig for begge gruppeområder (ikke koblet til en gruppe) og kommunikasjons område.</span><span class="sxs-lookup"><span data-stu-id="79050-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="79050-107">Flere funksjoner vil bli innført snart som gjør at du kan fortsette å bruke innholdet på området, men konvertere det eksisterende området til et område for kommunikasjon.</span><span class="sxs-lookup"><span data-stu-id="79050-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="79050-108">Disse evnene vil bli rullet ut gradvis.</span><span class="sxs-lookup"><span data-stu-id="79050-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="79050-109">Fortsett å sjekke Office 365 Message Center for oppdateringer.</span><span class="sxs-lookup"><span data-stu-id="79050-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="79050-110">Kjente problemer ved bytte av områder</span><span class="sxs-lookup"><span data-stu-id="79050-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="79050-111">Målområdet kan returnere en feilmelding av typen "ikke funnet" (HTTP 404) for en kort tidsperiode.</span><span class="sxs-lookup"><span data-stu-id="79050-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="79050-112">Innhold må være recrawled for å oppdatere søkeindeksen.</span><span class="sxs-lookup"><span data-stu-id="79050-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="79050-113">Det er ingen manuelle trinn som kreves-dette vil bli gjort automatisk.</span><span class="sxs-lookup"><span data-stu-id="79050-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="79050-114">Alt som er avhengig av "statiske" koblinger (for eksempel File Sync og OneNote-filer) må rettes manuelt.</span><span class="sxs-lookup"><span data-stu-id="79050-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="79050-115">Hvis kildeområdet var et organisatorisk nyhetsområde, oppdaterer du URL-adressen.</span><span class="sxs-lookup"><span data-stu-id="79050-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="79050-116">Få en liste over alle organisatoriske nyhetsnettsteder.</span><span class="sxs-lookup"><span data-stu-id="79050-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="79050-117">Project Server-områder må kanskje valideres for å sikre at de fortsatt er riktig tilknyttet.</span><span class="sxs-lookup"><span data-stu-id="79050-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





