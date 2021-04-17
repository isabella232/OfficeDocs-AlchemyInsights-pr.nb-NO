---
title: Feilsøke eksisterende skjerm
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824588"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="c5b56-102">Feilsøke en eksisterende skjerm</span><span class="sxs-lookup"><span data-stu-id="c5b56-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="c5b56-103">Prøv disse løsningene for å feilsøke en skjerm.</span><span class="sxs-lookup"><span data-stu-id="c5b56-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="c5b56-104">**Oppdater skjermens skjerm:**</span><span class="sxs-lookup"><span data-stu-id="c5b56-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="c5b56-105">Trykk følgende taster samtidig: Windows-tast + CTRL + SKIFT + B. Dette vil oppdatere kommunikasjonen med grafikkdriveren.</span><span class="sxs-lookup"><span data-stu-id="c5b56-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="c5b56-106">Skjermene blinker et øyeblikk og kommer tilbake etter noen sekunder.</span><span class="sxs-lookup"><span data-stu-id="c5b56-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="c5b56-107">**Feilsøke maskinvare for skjerm:**</span><span class="sxs-lookup"><span data-stu-id="c5b56-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="c5b56-108">Koble kabelen som kobler PC-en til skjermen, og koble den til igjen.</span><span class="sxs-lookup"><span data-stu-id="c5b56-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="c5b56-109">Koble alle ikke-essensielle enheter fra PC-en (for eksempel adaptere eller dokkingstasjoner).</span><span class="sxs-lookup"><span data-stu-id="c5b56-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="c5b56-110">**Hvis du nylig har installert en oppdatering på PC-en, kan du rulle tilbake skjermdriveren:**</span><span class="sxs-lookup"><span data-stu-id="c5b56-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="c5b56-111">Velg **Start**, skriv **inn enhetsbehandling**, og velg **Enhetsbehandling** fra resultatene.</span><span class="sxs-lookup"><span data-stu-id="c5b56-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="c5b56-112">Utvid **delen Skjermkort,** høyreklikk skjermkortet, og velg **Egenskaper**.</span><span class="sxs-lookup"><span data-stu-id="c5b56-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="c5b56-113">Gå til **Driver-fanen,** og velg **Rull tilbake driver**.</span><span class="sxs-lookup"><span data-stu-id="c5b56-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="c5b56-114">Obs! Hvis dette ikke er tilgjengelig eller  nedtonet, velger du Nei fra alternativene nedenfor for å gå til neste trinn.</span><span class="sxs-lookup"><span data-stu-id="c5b56-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="c5b56-115">Du må kanskje starte PC-en på nytt før disse endringene trer i kraft.</span><span class="sxs-lookup"><span data-stu-id="c5b56-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="c5b56-116">**Avinstaller skjermdriveren og installer den på nytt:**</span><span class="sxs-lookup"><span data-stu-id="c5b56-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="c5b56-117">Velg **Start**, skriv **inn enhetsbehandling**, og velg **Enhetsbehandling** fra resultatene.</span><span class="sxs-lookup"><span data-stu-id="c5b56-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="c5b56-118">Utvid **Delen Skjermkort,** høyreklikk skjermkortet, og velg **Avinstaller enhet**.</span><span class="sxs-lookup"><span data-stu-id="c5b56-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="c5b56-119">Velg boksen ved siden av **Slett driverprogramvaren for denne enheten,** og velg **Avinstaller**.</span><span class="sxs-lookup"><span data-stu-id="c5b56-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="c5b56-120">Obs! Du kan bli bedt om å starte datamaskinen på nytt på dette stadiet.</span><span class="sxs-lookup"><span data-stu-id="c5b56-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="c5b56-121">Pass på å skrive ned de gjenværende instruksjonene før du starter på nytt.</span><span class="sxs-lookup"><span data-stu-id="c5b56-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="c5b56-122">Åpne Enhetsbehandling på nytt.</span><span class="sxs-lookup"><span data-stu-id="c5b56-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="c5b56-123">Utvid **delen Skjermkort,** høyreklikk på skjermkortet, og velg **Oppdater driver**.</span><span class="sxs-lookup"><span data-stu-id="c5b56-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="c5b56-124">Velg **Søk automatisk etter oppdateringsdriverprogramvare,** og følg installasjonsinstruksjonene.</span><span class="sxs-lookup"><span data-stu-id="c5b56-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>