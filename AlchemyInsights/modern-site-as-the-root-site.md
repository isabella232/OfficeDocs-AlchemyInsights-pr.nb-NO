---
title: Moderne nettsted som rot område
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666879"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="cfd62-102">Moderne nettsted som rot område</span><span class="sxs-lookup"><span data-stu-id="cfd62-102">Modern site as root site</span></span>

<span data-ttu-id="cfd62-103">Vi har begynt å fremheve en ny funksjon som gjør at du kan [bytte til rot området for det klassiske nettstedet med et moderne nettsted](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="cfd62-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="cfd62-104">Bruk [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen til et nettsted med et annet område mens du arkiverer det opprinnelige nettstedet.</span><span class="sxs-lookup"><span data-stu-id="cfd62-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="cfd62-105">Tilgjengelig for både gruppe nettsted (ikke koblet til en gruppe) og kommunikasjons område.</span><span class="sxs-lookup"><span data-stu-id="cfd62-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="cfd62-106">Ikke slett det klassiske rot nettstedet for å opprette et moderne kommunikasjons område.</span><span class="sxs-lookup"><span data-stu-id="cfd62-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="cfd62-107">Dette støttes ikke av Microsoft.</span><span class="sxs-lookup"><span data-stu-id="cfd62-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="cfd62-108">Hvis du sletter rot området, blir alle SharePoint-nettsteder i organisasjonen utilgjengelig for alle brukere, til du gjenoppretter nettstedet eller oppretter et nytt nettsted på samme nett adresse.</span><span class="sxs-lookup"><span data-stu-id="cfd62-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="cfd62-109">Vi vil kommunisere denne funksjonen via meldings senteret.</span><span class="sxs-lookup"><span data-stu-id="cfd62-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="cfd62-110">Du bør også forvente at funksjonen skal slås på i leier snart.</span><span class="sxs-lookup"><span data-stu-id="cfd62-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="cfd62-111">Kjente problemer med å bytte nett steder</span><span class="sxs-lookup"><span data-stu-id="cfd62-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="cfd62-112">Mål området kan returnere en feil melding om at det ikke ble funnet (HTTP 404) i løpet av en kort tids periode.</span><span class="sxs-lookup"><span data-stu-id="cfd62-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="cfd62-113">Innhold må kravlesøkes for å oppdatere søke indeksen.</span><span class="sxs-lookup"><span data-stu-id="cfd62-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="cfd62-114">Det er ikke nødvendig med manuelt trinn, dette gjøres automatisk.</span><span class="sxs-lookup"><span data-stu-id="cfd62-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="cfd62-115">Alt som er avhengig av «statisk»-koblinger (for eksempel fil synkroniserings-og OneNote-filer), må korrigeres manuelt.</span><span class="sxs-lookup"><span data-stu-id="cfd62-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="cfd62-116">Project Server-områder må kanskje Valide res for å sikre at de fortsatt er riktige.</span><span class="sxs-lookup"><span data-stu-id="cfd62-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
