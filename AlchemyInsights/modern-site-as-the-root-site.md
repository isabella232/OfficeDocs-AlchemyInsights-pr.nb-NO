---
title: Moderne nettsted som rotstedet
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713800"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="66ab3-102">Moderne nettsted som rotnettsted</span><span class="sxs-lookup"><span data-stu-id="66ab3-102">Modern site as root site</span></span>

<span data-ttu-id="66ab3-103">Vi har begynt å rulle ut en ny funksjon som lar deg [bytte ditt klassiske nettsted rotnettsted med et moderne nettsted](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="66ab3-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="66ab3-104">Bruk [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen av et område med et annet område mens du arkiverer det opprinnelige området.</span><span class="sxs-lookup"><span data-stu-id="66ab3-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="66ab3-105">Tilgjengelig for både gruppeområde (ikke koblet til en gruppe) og kommunikasjonsområde.</span><span class="sxs-lookup"><span data-stu-id="66ab3-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="66ab3-106">Ikke slett det klassiske rotområdet for å opprette et moderne kommunikasjonsområde.</span><span class="sxs-lookup"><span data-stu-id="66ab3-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="66ab3-107">Dette støttes ikke av Microsoft.</span><span class="sxs-lookup"><span data-stu-id="66ab3-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="66ab3-108">Hvis du sletter rotområdet, blir alle SharePoint-områder i organisasjonen utilgjengelige for alle brukere, til du gjenoppretter området eller oppretter et nytt område på samme URL-adresse.</span><span class="sxs-lookup"><span data-stu-id="66ab3-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="66ab3-109">Vi kommuniserer denne funksjonen via meldingssenteret.</span><span class="sxs-lookup"><span data-stu-id="66ab3-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="66ab3-110">Du bør forvente at funksjonen skal slås på i leieren om kort tid.</span><span class="sxs-lookup"><span data-stu-id="66ab3-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="66ab3-111">Kjente problemer med bytte nettsteder</span><span class="sxs-lookup"><span data-stu-id="66ab3-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="66ab3-112">Målområdet kan returnere en "ikke funnet" (HTTP 404) feil i en kort periode.</span><span class="sxs-lookup"><span data-stu-id="66ab3-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="66ab3-113">Innholdet må søkes på nytt for å oppdatere søkeindeksen.</span><span class="sxs-lookup"><span data-stu-id="66ab3-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="66ab3-114">Det er ikke nødvendig med manuelt trinn her, dette vil bli gjort automatisk.</span><span class="sxs-lookup"><span data-stu-id="66ab3-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="66ab3-115">Alt som er avhengig av "statiske" koblinger (for eksempel Filsynkronisering og OneNote-filer), må korrigeres manuelt.</span><span class="sxs-lookup"><span data-stu-id="66ab3-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="66ab3-116">Project Server-områder må kanskje valideres for å sikre at de fortsatt er tilknyttet på riktig måte.</span><span class="sxs-lookup"><span data-stu-id="66ab3-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
