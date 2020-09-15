---
title: Dynamics 365 – feil instrument bord vises i Dynamics 365 Unified Interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711284"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="337d0-102">Feil instrument bord programmer vises i Dynamics 365 Unified Interface</span><span class="sxs-lookup"><span data-stu-id="337d0-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="337d0-103">Det finnes flere årsaker til at du kan se et annet instrument bord enn det du forventer:</span><span class="sxs-lookup"><span data-stu-id="337d0-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="337d0-104">Brukeren har angitt et standard instrument bord for bruker</span><span class="sxs-lookup"><span data-stu-id="337d0-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="337d0-105">Du kan vanligvis identifisere et bruker standard instrument bord som er angitt hvis **Angi som standard** -knappen ikke vises på instrument bord kommando linjen.</span><span class="sxs-lookup"><span data-stu-id="337d0-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="337d0-106">Bruker standard instrument bordet vil overstyre alle andre standard instrument bord, selv om brukerens standard instrument bord ikke er i gjeldende app.</span><span class="sxs-lookup"><span data-stu-id="337d0-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="337d0-107">Bruk følgende løsning for å fjerne standard instrument bord.</span><span class="sxs-lookup"><span data-stu-id="337d0-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="337d0-108">Opprette et nytt personlig instrument bord.</span><span class="sxs-lookup"><span data-stu-id="337d0-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="337d0-109">Angi at nytt instrument bord skal være standard for brukeren.</span><span class="sxs-lookup"><span data-stu-id="337d0-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="337d0-110">Slett dette instrument bordet.</span><span class="sxs-lookup"><span data-stu-id="337d0-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="337d0-111">Instrument bordet er angitt i Sitemap</span><span class="sxs-lookup"><span data-stu-id="337d0-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="337d0-112">Du kan ha angitt et standard instrument bord for organisasjonen ved å velge et instrument bord og velge angi som standard under Tilpass systemet.</span><span class="sxs-lookup"><span data-stu-id="337d0-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="337d0-113">Instrument bordet som er definert i kart-utforming-verktøyet, vil ha forrang over dette instrument bordet hvis brukeren har tilgang til det.</span><span class="sxs-lookup"><span data-stu-id="337d0-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="337d0-114">Hvis du vil at brukere skal se instrument bordet du har angitt som standard for organisasjonen, kan du enten:</span><span class="sxs-lookup"><span data-stu-id="337d0-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="337d0-115">Angi dette instrument bordet i område kart</span><span class="sxs-lookup"><span data-stu-id="337d0-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="337d0-116">Fjerne tilgang til det definerte instrument bord for sitemap for disse brukerne</span><span class="sxs-lookup"><span data-stu-id="337d0-116">Remove access to the sitemap defined dashboard for those users</span></span>
