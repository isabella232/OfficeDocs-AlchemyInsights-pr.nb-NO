---
title: Skrivebeskyttet for vedlikehold-melding når du prøver å bruke SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051290"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="5b15f-102">Skrivebeskyttet for vedlikehold-melding når du prøver å bruke SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="5b15f-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="5b15f-103">Brukere kan få en **skrivebeskyttet for vedlikehold** melding når du prøver å bruke SharePoint eller OneDrive for ett av følgende scenarier.</span><span class="sxs-lookup"><span data-stu-id="5b15f-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="5b15f-104">En planlagt eller aktiv vedlikeholdsaktivitet.</span><span class="sxs-lookup"><span data-stu-id="5b15f-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="5b15f-105">Se etter dem ved å navigere til [meldingssenteret](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="5b15f-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="5b15f-106">En høyt prioritert, aktiv service-hendelse som kan inntreffe.</span><span class="sxs-lookup"><span data-stu-id="5b15f-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="5b15f-107">Se etter eventuelle veiledninger/hendelser ved å navigere til [service Health](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="5b15f-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="5b15f-108">En mindre Auto-healing utvinning scenario som kan skje på grunn av uventede hendelser på servere som kan vare i mindre enn 30 min eller så.</span><span class="sxs-lookup"><span data-stu-id="5b15f-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="5b15f-109">Det er ingen Message Center eller service Health innlegg for disse mindre inngang, men du bør være tilbake til normal ganske snart.</span><span class="sxs-lookup"><span data-stu-id="5b15f-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="5b15f-110">Opp på svært få anledninger vi bemerket det ettall av det tre filmmanuskriptet katalogiseret over ha blitt årsaken, og service er blitt gjenopprettet, bortsett fra det brukernes kikker skjulested har ikke ' blitt klarnet opp.</span><span class="sxs-lookup"><span data-stu-id="5b15f-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="5b15f-111">Prøv å tømme nettleserens hurtigbuffer før du navigerer til området.</span><span class="sxs-lookup"><span data-stu-id="5b15f-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="5b15f-112">Velg **Innstillinger**i Microsoft Edge-nettleseren, og velg deretter **personvern og sikkerhet**.</span><span class="sxs-lookup"><span data-stu-id="5b15f-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="5b15f-113">Under **fjernnett lesing**velger **du Velg hva du vil fjerne**.</span><span class="sxs-lookup"><span data-stu-id="5b15f-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="5b15f-114">Velg **informasjonskapsler og lagrede nettstedsdata**, og velg **Fjern**.</span><span class="sxs-lookup"><span data-stu-id="5b15f-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="5b15f-115">Disse trinnene kan variere når du bruker andre nettlesere, for eksempel Mozilla Firefox eller Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="5b15f-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="5b15f-116">Et annet alternativ er å åpne SharePoint-området eller OneDrive i et nytt InPrivate-vindu.</span><span class="sxs-lookup"><span data-stu-id="5b15f-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>