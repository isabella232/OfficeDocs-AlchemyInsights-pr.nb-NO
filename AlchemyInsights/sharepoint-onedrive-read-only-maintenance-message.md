---
title: Skrivebeskyttet for vedlikehold melding når du prøver å bruke SharePoint- eller OneDrive
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620732"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="07859-102">Skrivebeskyttet for vedlikehold melding når du prøver å bruke SharePoint- eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="07859-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="07859-103">Brukere kan få en **Skrivebeskyttet for vedlikehold** melding når du prøver å bruke SharePoint- eller OneDrive for ett av følgende scenarier.</span><span class="sxs-lookup"><span data-stu-id="07859-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="07859-104">En aktivitet planlagt eller aktiv vedlikehold.</span><span class="sxs-lookup"><span data-stu-id="07859-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="07859-105">Se etter dem ved å navigere til [Meldingssentral](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="07859-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="07859-106">En høy prioritet, aktive tjenesten problemer som kan oppstå.</span><span class="sxs-lookup"><span data-stu-id="07859-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="07859-107">Se etter eventuelle veiledningene/hendelser ved å navigere til [Health Service](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="07859-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="07859-108">Et mindre automatisk reparasjon gjenoppretting scenario som kan skje på grunn av uventede hendelser på servere som kan vare i mindre enn 30 minutter eller så.</span><span class="sxs-lookup"><span data-stu-id="07859-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="07859-109">Det finnes ingen Message Center eller tjenesten helse bokfører disse underordnede gjenopprettinger, men du bør være tilbake til normal veldig snart.</span><span class="sxs-lookup"><span data-stu-id="07859-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="07859-110">Vi observerte at én av tre scenariene ovenfor er årsaken, og tjenesten er gjenopprettet, men hurtigbufferen for webleseren brukere ikke har blitt tømt i svært få tilfeller.</span><span class="sxs-lookup"><span data-stu-id="07859-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="07859-111">Prøv å tømme hurtigbufferen for webleseren før du navigere til området.</span><span class="sxs-lookup"><span data-stu-id="07859-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="07859-112">I webleseren Microsoft Edge, velg **Innstillinger**, og velg deretter **Personvern og sikkerhet**.</span><span class="sxs-lookup"><span data-stu-id="07859-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="07859-113">**Fjern Bla gjennom**, velg **Velg hva du vil fjerne**.</span><span class="sxs-lookup"><span data-stu-id="07859-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="07859-114">Velg **informasjonskapsler og webområdet for lagrede data**, og velg **Fjern**.</span><span class="sxs-lookup"><span data-stu-id="07859-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="07859-115">Disse trinnene kan variere når du bruker andre lesere, for eksempel Mozilla Firefox eller Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="07859-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="07859-116">Et annet alternativ er å åpne SharePoint-området eller OneDrive i et nytt InPrivate-vindu.</span><span class="sxs-lookup"><span data-stu-id="07859-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>