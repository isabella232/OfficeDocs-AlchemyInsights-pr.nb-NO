---
title: Bytte ut det klassiske rot området med et moderne nettsted
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691188"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="d4762-102">Bytte ut det klassiske rot området med et moderne nettsted</span><span class="sxs-lookup"><span data-stu-id="d4762-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="d4762-103">Hvis miljøet ble konfigurert før 2019, kan du endre rot nettstedet til et moderne nettsted ved hjelp av Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="d4762-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="d4762-104">Hvis du har et annet nettsted du vil bruke som rot område, kan du erstatte [(bytte) det primære nettstedet](https://docs.microsoft.com/sharepoint/modern-root-site) med det.</span><span class="sxs-lookup"><span data-stu-id="d4762-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="d4762-105">Bruk [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen til et nettsted med et annet område mens du arkiverer det opprinnelige nettstedet.</span><span class="sxs-lookup"><span data-stu-id="d4762-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="d4762-106">Tilgjengelig for både gruppe nettsted (ikke koblet til en gruppe) og kommunikasjons område.</span><span class="sxs-lookup"><span data-stu-id="d4762-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="d4762-107">Flere funksjoner kommer snart til at du kan fortsette å bruke innholdet på området, men konvertere det eksisterende nettstedet til et kommunikasjons område.</span><span class="sxs-lookup"><span data-stu-id="d4762-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="d4762-108">Disse funksjonene blir rullet ut gradvis.</span><span class="sxs-lookup"><span data-stu-id="d4762-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="d4762-109">Fortsett å kontrollere meldings senteret for oppdateringer.</span><span class="sxs-lookup"><span data-stu-id="d4762-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="d4762-110">Kjente problemer med å bytte nett steder</span><span class="sxs-lookup"><span data-stu-id="d4762-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="d4762-111">Mål området kan returnere en feil melding om at det ikke ble funnet (HTTP 404) i løpet av en kort tids periode.</span><span class="sxs-lookup"><span data-stu-id="d4762-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="d4762-112">Innhold må kravlesøkes for å oppdatere søke indeksen.</span><span class="sxs-lookup"><span data-stu-id="d4762-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="d4762-113">Det er ikke nødvendig med et manuelt trinn – dette skjer automatisk.</span><span class="sxs-lookup"><span data-stu-id="d4762-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="d4762-114">Alt som er avhengig av «statisk»-koblinger (for eksempel fil synkroniserings-og OneNote-filer), må korrigeres manuelt.</span><span class="sxs-lookup"><span data-stu-id="d4762-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="d4762-115">Hvis kilde området var et organisasjons nyhets nettsted, oppdaterer du URL-adressen.</span><span class="sxs-lookup"><span data-stu-id="d4762-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="d4762-116">Få en liste over alle organisasjonens nyhets områder.</span><span class="sxs-lookup"><span data-stu-id="d4762-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="d4762-117">Project Server-områder må kanskje Valide res for å sikre at de fortsatt er riktige.</span><span class="sxs-lookup"><span data-stu-id="d4762-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
