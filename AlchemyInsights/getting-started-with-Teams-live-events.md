---
title: Komme i gang med Teams og live-hendelser
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000208"
- "3436"
ms.openlocfilehash: a10f756fc69a7a135446d8d3bcec1f5e951627d8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811969"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="26d1a-102">Komme i gang med Teams og live-hendelser</span><span class="sxs-lookup"><span data-stu-id="26d1a-102">Getting started with Teams live events</span></span>

<span data-ttu-id="26d1a-103">Microsoft Teams Live-hendelser er en utvidelse av Teams-møter, som gjør det mulig for deg å planlegge og produsere hendelser som direkteavspilles mot store nettbaserte målgrupper.</span><span class="sxs-lookup"><span data-stu-id="26d1a-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="26d1a-104">For å opprette en live-hendelse trenger du følgende:</span><span class="sxs-lookup"><span data-stu-id="26d1a-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="26d1a-105">Først må du kontrollere at Direktesendte teams-arrangementer [er tilgjengelige i ditt land og område](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability). Direktesendte arrangementer støttes ennå ikke i enkelte land.</span><span class="sxs-lookup"><span data-stu-id="26d1a-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="26d1a-106">Hvis du har tilordnet lisenser og angitt policyer, men fremdeles ikke kan opprette et Teams Live-arrangement, er det sannsynlig at du er i et land eller område der direktesendte arrangementer ennå ikke er tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="26d1a-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="26d1a-107">En [Office 365 Enterprise E1-, E3-eller E5-lisens eller en Office-365 A3-eller A5-lisens](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="26d1a-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="26d1a-108">**Merk**: på grunn av en nylig økning i bruken av Teams kan det ta omtrent 24 timer før alt er ordentlig satt opp etter at du har gitt en lisens til en bruker.</span><span class="sxs-lookup"><span data-stu-id="26d1a-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="26d1a-109">Frem til det kan du ikke tilordne Teams-policyer til dem, og det kan hende de ikke har tilgang til enkelte Teams-funksjoner som anrop og lydkonferanser.</span><span class="sxs-lookup"><span data-stu-id="26d1a-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="26d1a-110">Tillatelse til å [opprette live-hendelser i administrasjonssenteret for Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span><span class="sxs-lookup"><span data-stu-id="26d1a-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="26d1a-111">Tillatelse til å [opprette live-hendelser i Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for hendelser som produseres ved bruk av en ekstern kringkastingsapp eller enhet).</span><span class="sxs-lookup"><span data-stu-id="26d1a-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="26d1a-112">Fullstendig gruppemedlemskap i organisasjonen (kan ikke være en gjest eller fra en annen organisasjon).</span><span class="sxs-lookup"><span data-stu-id="26d1a-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="26d1a-113">Privat møtetidsplan, skjermdeling og deling av IP-video, aktivert i gruppemøtepolicyen.</span><span class="sxs-lookup"><span data-stu-id="26d1a-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="26d1a-114">[Anbefalte fremgangsmåter](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams live-hendelser.</span><span class="sxs-lookup"><span data-stu-id="26d1a-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="26d1a-115">Hvis du vil ha mer informasjon, kan du se [Komme i gang med Microsoft Teams Live-hendelser](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span><span class="sxs-lookup"><span data-stu-id="26d1a-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>