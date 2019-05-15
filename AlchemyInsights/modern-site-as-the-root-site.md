---
title: Moderne området som det primære området
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057747"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="25202-102">Moderne område som rotområde</span><span class="sxs-lookup"><span data-stu-id="25202-102">Modern site as root site</span></span>

<span data-ttu-id="25202-103">[Utgivelsen av mål](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) kunder kan nå aktivere moderne kommunikasjon området opplevelse på klassisk rotområdet for sine SharePoint leier.</span><span class="sxs-lookup"><span data-stu-id="25202-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="25202-104">Denne funksjonen kan aktiveres ved å kjøre en enkel PowerShell-cmdleten.</span><span class="sxs-lookup"><span data-stu-id="25202-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="25202-105">For vellykket kjøring av PowerShell-kommandoer må det primære området en ny kommunikasjon-hjemmesiden.</span><span class="sxs-lookup"><span data-stu-id="25202-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="25202-106">Detaljer om kravene til PowerShell-cmdlet og funksjonen er tilgjengelig i artikkelen [Aktivere SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="25202-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="25202-107">Vi vil bli gradvis rullende dette ut, av som standard til angitt versjon kunder i tidlig mai 2019, og Rull ut vil være tilgjengelig over hele verden på slutten av juni 2019.</span><span class="sxs-lookup"><span data-stu-id="25202-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="25202-108">Fortsette å referere til [Meldingssentral](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for andre nye funksjoner med moderne.</span><span class="sxs-lookup"><span data-stu-id="25202-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="25202-109">**Viktig**: ikke Slett klassisk rotområdet for å opprette et område for moderne kommunikasjon.</span><span class="sxs-lookup"><span data-stu-id="25202-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="25202-110">Dette støttes ikke av Microsoft.</span><span class="sxs-lookup"><span data-stu-id="25202-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="25202-111">Sletter det primære området, blir alle SharePoint-områder i organisasjonen utilgjengelig for alle brukere, før du kan gjenopprette området eller opprette et nytt område på den samme URL-adressen.</span><span class="sxs-lookup"><span data-stu-id="25202-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 