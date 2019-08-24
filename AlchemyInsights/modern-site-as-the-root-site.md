---
title: Moderne området som det primære området
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: d5ea73c967013822854dbd408d4628d991c90378
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620768"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="fcbdf-102">Moderne område som rotområde</span><span class="sxs-lookup"><span data-stu-id="fcbdf-102">Modern site as root site</span></span>

<span data-ttu-id="fcbdf-103">Vi har begynt å utrullingen en ny funksjon som lar deg bytte rotområdet klassisk område med et moderne område.</span><span class="sxs-lookup"><span data-stu-id="fcbdf-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="fcbdf-104">Bruk [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen av et område med et annet område under arkivering av det opprinnelige området.</span><span class="sxs-lookup"><span data-stu-id="fcbdf-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="fcbdf-105">Tilgjengelig for både Team (ikke koblet til en gruppe) og kommunikasjon-området.</span><span class="sxs-lookup"><span data-stu-id="fcbdf-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="fcbdf-106">Ikke Slett klassisk rotområdet for å opprette et område for moderne kommunikasjon.</span><span class="sxs-lookup"><span data-stu-id="fcbdf-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="fcbdf-107">Dette støttes ikke av Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fcbdf-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="fcbdf-108">Sletter det primære området, blir alle SharePoint-områder i organisasjonen utilgjengelig for alle brukere, før du kan gjenopprette området eller opprette et nytt område på den samme URL-adressen.</span><span class="sxs-lookup"><span data-stu-id="fcbdf-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="fcbdf-109">Vi skal kommunisere denne funksjonen via Meldingssentret.</span><span class="sxs-lookup"><span data-stu-id="fcbdf-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="fcbdf-110">Du bør forvente at funksjonen skal være aktivert i din leier kort tid.</span><span class="sxs-lookup"><span data-stu-id="fcbdf-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="fcbdf-111">Kjente problemer med bytte områder</span><span class="sxs-lookup"><span data-stu-id="fcbdf-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="fcbdf-112">Målområdet kan returnere en "not found" (HTTP 404)-feil for en kort tidsperiode.</span><span class="sxs-lookup"><span data-stu-id="fcbdf-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="fcbdf-113">Innhold må være kravlesøkt på nytt for å oppdatere søkeindeksen.</span><span class="sxs-lookup"><span data-stu-id="fcbdf-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="fcbdf-114">Det er ingen manuelle trinn nødvendig her, dette vil bli gjort automatisk.</span><span class="sxs-lookup"><span data-stu-id="fcbdf-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="fcbdf-115">Alt avhengig av "statisk" koblinger (for eksempel filsynkronisering og OneNote-filer) må korrigeres manuelt.</span><span class="sxs-lookup"><span data-stu-id="fcbdf-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="fcbdf-116">Project Server-områder må kanskje valideres for å sikre at de er fortsatt tilknyttet på riktig måte.</span><span class="sxs-lookup"><span data-stu-id="fcbdf-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
