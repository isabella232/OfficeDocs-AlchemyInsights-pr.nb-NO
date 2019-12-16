---
title: Moderne område som roten området
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054711"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="185b9-102">Moderne nettsted som root nettsted</span><span class="sxs-lookup"><span data-stu-id="185b9-102">Modern site as root site</span></span>

<span data-ttu-id="185b9-103">Vi har begynt å utrulling en ny funksjon som vil tillate deg å [bytte din klassiske nettstedet root nettsted med et moderne nettsted](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="185b9-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="185b9-104">Bruk [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen av et område med et annet område under arkivering av det opprinnelige området.</span><span class="sxs-lookup"><span data-stu-id="185b9-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="185b9-105">Tilgjengelig for begge gruppeområder (ikke koblet til en gruppe) og kommunikasjons område.</span><span class="sxs-lookup"><span data-stu-id="185b9-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="185b9-106">Ikke slett det klassiske rotområdet for å opprette et moderne kommunikasjons nettsted.</span><span class="sxs-lookup"><span data-stu-id="185b9-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="185b9-107">Dette støttes ikke av Microsoft.</span><span class="sxs-lookup"><span data-stu-id="185b9-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="185b9-108">Hvis du sletter rotområdet, vil alle SharePoint-områder i organisasjonen være utilgjengelige for alle brukere, helt til du gjenoppretter området eller oppretter et nytt område på samme URL-adresse.</span><span class="sxs-lookup"><span data-stu-id="185b9-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="185b9-109">Vi kommuniserer denne funksjonen via meldingssentralen.</span><span class="sxs-lookup"><span data-stu-id="185b9-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="185b9-110">Du bør forvente at funksjonen skal være slått på i leietaker kort tid.</span><span class="sxs-lookup"><span data-stu-id="185b9-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="185b9-111">Kjente problemer ved bytte av områder</span><span class="sxs-lookup"><span data-stu-id="185b9-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="185b9-112">Målområdet kan returnere en feilmelding av typen "ikke funnet" (HTTP 404) for en kort tidsperiode.</span><span class="sxs-lookup"><span data-stu-id="185b9-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="185b9-113">Innhold må være recrawled for å oppdatere søkeindeksen.</span><span class="sxs-lookup"><span data-stu-id="185b9-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="185b9-114">Det er ingen manuelle trinn som kreves her, dette vil bli gjort automatisk.</span><span class="sxs-lookup"><span data-stu-id="185b9-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="185b9-115">Alt som er avhengig av "statiske" koblinger (for eksempel File Sync og OneNote-filer) må rettes manuelt.</span><span class="sxs-lookup"><span data-stu-id="185b9-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="185b9-116">Project Server-områder må kanskje valideres for å sikre at de fortsatt er riktig tilknyttet.</span><span class="sxs-lookup"><span data-stu-id="185b9-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
