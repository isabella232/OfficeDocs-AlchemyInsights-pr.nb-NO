---
title: Dynamics 365 - feil instrumentbord viser i Dynamics 365 enhetlig grensesnitt
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528560"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="27bad-102">Viser feil instrumentbord i Dynamics 365 enhetlig grensesnitt</span><span class="sxs-lookup"><span data-stu-id="27bad-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="27bad-103">Det er flere grunner til hvorfor du kanskje se en annen instrumentbord enn den du forventer:</span><span class="sxs-lookup"><span data-stu-id="27bad-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="27bad-104">Brukeren har angitt en bruker standard instrumentbord</span><span class="sxs-lookup"><span data-stu-id="27bad-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="27bad-105">Vanligvis kan du identifisere en bruker standard instrumentbord er angitt Hvis knappen **Angi som standard** ikke vises i kommandolinjen for instrumentbordet.</span><span class="sxs-lookup"><span data-stu-id="27bad-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="27bad-106">Bruker standard instrumentbord overstyrer alle andre instrumentbord for standard selv om brukerens standard instrumentbord ikke er i gjeldende program.</span><span class="sxs-lookup"><span data-stu-id="27bad-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="27bad-107">Bruk følgende løsning å Fjern deres standard instrumentbord.</span><span class="sxs-lookup"><span data-stu-id="27bad-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="27bad-108">Opprett et nytt personlig instrumentbord.</span><span class="sxs-lookup"><span data-stu-id="27bad-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="27bad-109">Angi det nye instrumentbordet som Brukerstandard.</span><span class="sxs-lookup"><span data-stu-id="27bad-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="27bad-110">Slett dette instrumentbordet.</span><span class="sxs-lookup"><span data-stu-id="27bad-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="27bad-111">Instrumentbordet er satt i områdekartet</span><span class="sxs-lookup"><span data-stu-id="27bad-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="27bad-112">Du har angitt en standard instrumentbord for organisasjonen ved å velge et instrumentbord og velge "Angi som standard, under Tilpass i systemet.</span><span class="sxs-lookup"><span data-stu-id="27bad-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="27bad-113">Men instrumentbord som er definert i sitemap designer skal prioriteres foran dette instrumentbordet Hvis brukeren har tilgang til den.</span><span class="sxs-lookup"><span data-stu-id="27bad-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="27bad-114">Hvis du vil at brukere kan vise instrumentbordet du har angitt som Organisasjonsstandard, kan du:</span><span class="sxs-lookup"><span data-stu-id="27bad-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="27bad-115">Angi dette instrumentbordet i områdekartet</span><span class="sxs-lookup"><span data-stu-id="27bad-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="27bad-116">Fjern tilgang til instrumentbordet sitemap som er definert for disse brukerne</span><span class="sxs-lookup"><span data-stu-id="27bad-116">Remove access to the sitemap defined dashboard for those users</span></span>
