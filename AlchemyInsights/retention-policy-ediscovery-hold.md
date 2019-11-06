---
title: 2609-oppbevaring-eller-eDiscovery-Hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994082"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="0b8ca-102">Kan ikke slette elementer i SharePoint Online eller OneDrive for bedrifter</span><span class="sxs-lookup"><span data-stu-id="0b8ca-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="0b8ca-103">Du eller brukerne kan ikke slette elementer i SharePoint Online eller OneDrive for bedrifter fordi en oppbevaringspolicy, oppbevaring etikett eller eDiscovery holder brukes på et SharePoint-område for OneDrive eller et bestemt element.</span><span class="sxs-lookup"><span data-stu-id="0b8ca-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="0b8ca-104">Dette inkluderer at du ikke kan slette et dokument, en dokumentversjon, en mappe, et dokumentbibliotek, en liste, en app, et område eller en områdesamling.</span><span class="sxs-lookup"><span data-stu-id="0b8ca-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="0b8ca-105">Her er noen eksempler på feilmeldinger du kan motta hvis du prøver å slette et element som beholdes:</span><span class="sxs-lookup"><span data-stu-id="0b8ca-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="0b8ca-106">"Dette området kan ikke slettes fordi det er inkludert i en eDiscovery holder eller oppbevaringspolicy"</span><span class="sxs-lookup"><span data-stu-id="0b8ca-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="0b8ca-107">"Dette området har en samsvars policy som er satt til å blokkere sletting"</span><span class="sxs-lookup"><span data-stu-id="0b8ca-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="0b8ca-108">"En samsvars policy blokkerer for øyeblikket slettingen av dette området"</span><span class="sxs-lookup"><span data-stu-id="0b8ca-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="0b8ca-109">"Denne områdesamlingen kan ikke slettes fordi den inneholder områder som er inkludert i en eDiscovery holder eller oppbevaringspolicy"</span><span class="sxs-lookup"><span data-stu-id="0b8ca-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="0b8ca-110">"Du må slette alle elementene i denne mappen før du sletter mappen"</span><span class="sxs-lookup"><span data-stu-id="0b8ca-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="0b8ca-111">"Versjoner av dette elementet kan ikke slettes fordi det er på vent eller oppbevaringspolicy"</span><span class="sxs-lookup"><span data-stu-id="0b8ca-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="0b8ca-112">"Elementet kan ikke slettes mens du er på vent"</span><span class="sxs-lookup"><span data-stu-id="0b8ca-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="0b8ca-113">"Etiketten som brukes på dette elementet, hindrer den i å redigeres eller slettes"</span><span class="sxs-lookup"><span data-stu-id="0b8ca-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="0b8ca-114">"Listen kan ikke slettes når du er på vent eller oppbevaringspolicy"</span><span class="sxs-lookup"><span data-stu-id="0b8ca-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="0b8ca-115">"Listen kan ikke slettes hvis den er blokkert, eller hvis en oppbevaringspolicy brukes på den"</span><span class="sxs-lookup"><span data-stu-id="0b8ca-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="0b8ca-116">For å slette elementer i ett av disse scenariene må oppbevaringspolicyen, oppbevarings etiketten eller eDiscovery-tak fjernes (eller et område må utelates fra en oppbevaringspolicy).</span><span class="sxs-lookup"><span data-stu-id="0b8ca-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="0b8ca-117">Du må enten deaktivere eller ekskludere respektive hold som forårsaker dette problemet.</span><span class="sxs-lookup"><span data-stu-id="0b8ca-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="0b8ca-118">Etter at en oppbevaringspolicy eller et Hold er fjernet, kan det ta opptil 24 timer for endringen trer i kraft.</span><span class="sxs-lookup"><span data-stu-id="0b8ca-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="0b8ca-119">Hvis du vil ha informasjon om de forskjellige funksjonene for oppbevaring og hold som kan brukes på SharePoint-områder og OneDrive-kontoer, se ett av følgende emner.</span><span class="sxs-lookup"><span data-stu-id="0b8ca-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="0b8ca-120">Oversikt over oppbevaringspolicyer</span><span class="sxs-lookup"><span data-stu-id="0b8ca-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="0b8ca-121">Oversikt over oppbevarings etiketter</span><span class="sxs-lookup"><span data-stu-id="0b8ca-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="0b8ca-122">Behandle sperringer i avansert eDiscovery</span><span class="sxs-lookup"><span data-stu-id="0b8ca-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="0b8ca-123">eDiscovery inneholder</span><span class="sxs-lookup"><span data-stu-id="0b8ca-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="0b8ca-124">Retningslinjer for avslutning og sletting av eldre områder</span><span class="sxs-lookup"><span data-stu-id="0b8ca-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
