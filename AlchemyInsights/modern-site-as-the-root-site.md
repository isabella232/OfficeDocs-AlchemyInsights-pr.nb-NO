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
ms.openlocfilehash: 260048db6c439183da8e0bb0c2dfa3c7475fca79
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269385"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="63cc3-102">Moderne område som rotområde</span><span class="sxs-lookup"><span data-stu-id="63cc3-102">Modern site as root site</span></span>

<span data-ttu-id="63cc3-103">Vi har begynt å utrullingen en ny funksjon som lar deg bytte rotområdet klassisk område med et moderne område.</span><span class="sxs-lookup"><span data-stu-id="63cc3-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="63cc3-104">Bruk [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen av et område med et annet område under arkivering av det opprinnelige området.</span><span class="sxs-lookup"><span data-stu-id="63cc3-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="63cc3-105">Tilgjengelig for både Team (ikke koblet til en gruppe) og kommunikasjon-området.</span><span class="sxs-lookup"><span data-stu-id="63cc3-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="63cc3-106">Ikke Slett klassisk rotområdet for å opprette et område for moderne kommunikasjon.</span><span class="sxs-lookup"><span data-stu-id="63cc3-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="63cc3-107">Dette støttes ikke av Microsoft.</span><span class="sxs-lookup"><span data-stu-id="63cc3-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="63cc3-108">Sletter det primære området, blir alle SharePoint-områder i organisasjonen utilgjengelig for alle brukere, før du kan gjenopprette området eller opprette et nytt område på den samme URL-adressen.</span><span class="sxs-lookup"><span data-stu-id="63cc3-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="63cc3-109">Vi skal kommunisere denne funksjonen via Meldingssentret.</span><span class="sxs-lookup"><span data-stu-id="63cc3-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="63cc3-110">Du bør forvente at funksjonen skal være aktivert i din leier kort tid.</span><span class="sxs-lookup"><span data-stu-id="63cc3-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="63cc3-111">Kjente problemer med bytte områder</span><span class="sxs-lookup"><span data-stu-id="63cc3-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="63cc3-112">Målområdet kan returnere en "not found" (HTTP 404)-feil for en kort tidsperiode.</span><span class="sxs-lookup"><span data-stu-id="63cc3-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="63cc3-113">Innhold må være kravlesøkt på nytt for å oppdatere søkeindeksen.</span><span class="sxs-lookup"><span data-stu-id="63cc3-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="63cc3-114">Det er ingen manuelle trinn nødvendig her, dette vil bli gjort automatisk.</span><span class="sxs-lookup"><span data-stu-id="63cc3-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="63cc3-115">Alt avhengig av "statisk" koblinger (for eksempel filsynkronisering og OneNote-filer) må korrigeres manuelt.</span><span class="sxs-lookup"><span data-stu-id="63cc3-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="63cc3-116">Project Server-områder må kanskje valideres for å sikre at de er fortsatt tilknyttet på riktig måte.</span><span class="sxs-lookup"><span data-stu-id="63cc3-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
