---
title: Dynamics 365-feil Dashboard viser i Dynamics 365 enhetlig grensesnitt
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528560"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="35297-102">Feil dashbord vises i Dynamics 365 enhetlig grensesnitt</span><span class="sxs-lookup"><span data-stu-id="35297-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="35297-103">Det kan være flere grunner til at du ser et annet instrumentbord enn det du forventer:</span><span class="sxs-lookup"><span data-stu-id="35297-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="35297-104">Brukeren har angitt et standard instrumentbord for bruker</span><span class="sxs-lookup"><span data-stu-id="35297-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="35297-105">Vanligvis kan du identifisere en brukers standard instrumentbord er angitt hvis **angitt som standard** -knappen ikke vises i kommandolinjen for instrumentbordet.</span><span class="sxs-lookup"><span data-stu-id="35297-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="35297-106">Bruker standard instrumentbord overstyrer alle andre standard instrumentbord, selv om brukerens standard instrumentbord ikke er i den gjeldende appen.</span><span class="sxs-lookup"><span data-stu-id="35297-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="35297-107">Bruk følgende løsning for å avbryte Standardinstrumentbordet.</span><span class="sxs-lookup"><span data-stu-id="35297-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="35297-108">Opprett et nytt personlig instrumentbord.</span><span class="sxs-lookup"><span data-stu-id="35297-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="35297-109">Angi det nye instrumentbordet som bruker standard.</span><span class="sxs-lookup"><span data-stu-id="35297-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="35297-110">Slett dette instrumentbordet.</span><span class="sxs-lookup"><span data-stu-id="35297-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="35297-111">Dashbordet er satt i Sitemap</span><span class="sxs-lookup"><span data-stu-id="35297-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="35297-112">Du kan ha angitt et standard instrumentbord for organisasjonen ved å velge et instrumentbord og velge angi som standard under Tilpass systemet.</span><span class="sxs-lookup"><span data-stu-id="35297-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="35297-113">Men dashbordet definert i Sitemap designeren vil forrang over dette dashbordet, hvis brukeren har tilgang til den.</span><span class="sxs-lookup"><span data-stu-id="35297-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="35297-114">Hvis du vil at brukerne skal se instrumentbordet du har angitt som organisasjonsstandard, kan du gjøre ett av følgende:</span><span class="sxs-lookup"><span data-stu-id="35297-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="35297-115">Angi dette instrumentbordet i områdekartet</span><span class="sxs-lookup"><span data-stu-id="35297-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="35297-116">Fjern tilgangen til sitemap-definerte dashbord for disse brukerne</span><span class="sxs-lookup"><span data-stu-id="35297-116">Remove access to the sitemap defined dashboard for those users</span></span>
