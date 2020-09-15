---
title: Skrivebeskyttet for vedlikeholds melding når du prøver å bruke SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670841"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="08300-102">Skrivebeskyttet for vedlikeholds melding når du prøver å bruke SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="08300-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="08300-103">Brukere kan motta en **skrivebeskyttet for vedlikeholds** melding når du prøver å bruke SharePoint eller OneDrive for ett av følgende scenarioer.</span><span class="sxs-lookup"><span data-stu-id="08300-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="08300-104">En planlagt eller aktiv vedlikeholds aktivitet.</span><span class="sxs-lookup"><span data-stu-id="08300-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="08300-105">Se etter dem ved å navigere til [meldings senteret](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="08300-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="08300-106">En aktiv tjeneste hendelse med høy prioritet, som kan oppstå.</span><span class="sxs-lookup"><span data-stu-id="08300-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="08300-107">Se etter en rådgiver/hendelser ved å navigere til [tjeneste tilstand](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="08300-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="08300-108">Et mindre scenario for automatisk reparasjons gjenoppretting som kan oppstå på grunn av eventuelle uventede hendelser på serverne som kanskje har mindre enn 30 min eller så videre.</span><span class="sxs-lookup"><span data-stu-id="08300-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="08300-109">Det finnes ingen inn Legg for meldings senter eller tjeneste tilstander for disse underordnede oppmøtene, men du bør snart gå tilbake til normal.</span><span class="sxs-lookup"><span data-stu-id="08300-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="08300-110">I svært få tilfeller observerte vi at et av de tre scenariene som er oppført ovenfor, har vært årsaken, og at tjenesten er gjen opprettet, men brukernes nett leser buffer er ikke tømt.</span><span class="sxs-lookup"><span data-stu-id="08300-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="08300-111">Prøv å tømme nett leser bufferen før du navigerer til området.</span><span class="sxs-lookup"><span data-stu-id="08300-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="08300-112">Velg **Innstillinger**i Microsoft Edge-leseren, og velg deretter **person vern og sikkerhet**.</span><span class="sxs-lookup"><span data-stu-id="08300-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="08300-113">Under **Tøm nett lesing**velger **du Velg hva som skal fjernes**.</span><span class="sxs-lookup"><span data-stu-id="08300-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="08300-114">Velg **informasjons kapsler og lagrede nettsteds data**, og velg **Fjern**.</span><span class="sxs-lookup"><span data-stu-id="08300-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="08300-115">Disse trinnene kan variere når du bruker andre nett lesere, for eksempel Mozilla Firefox eller Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="08300-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="08300-116">Et annet alternativ vil være å åpne SharePoint-området eller OneDrive i et nytt InPrivate-vindu.</span><span class="sxs-lookup"><span data-stu-id="08300-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>