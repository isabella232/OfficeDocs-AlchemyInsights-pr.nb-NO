---
title: Feilsøke eksisterende skjerm
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690720"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="96a19-102">Feilsøke en eksisterende skjerm</span><span class="sxs-lookup"><span data-stu-id="96a19-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="96a19-103">Prøv disse løsningene for å feilsøke en skjerm.</span><span class="sxs-lookup"><span data-stu-id="96a19-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="96a19-104">**Oppdater skjermens skjerm:**</span><span class="sxs-lookup"><span data-stu-id="96a19-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="96a19-105">Trykk følgende taster på samme tid: Windows-tast + Ctrl + Skift + B. Dette vil oppdatere kommunikasjonen med grafikk drive ren.</span><span class="sxs-lookup"><span data-stu-id="96a19-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="96a19-106">Skjermene blinker på en liten stund og kommer tilbake etter noen sekunder.</span><span class="sxs-lookup"><span data-stu-id="96a19-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="96a19-107">**Feilsøke overvåking av maskin vare:**</span><span class="sxs-lookup"><span data-stu-id="96a19-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="96a19-108">Koble fra kabelen som kobler PC-en til skjermen, og koble den til igjen.</span><span class="sxs-lookup"><span data-stu-id="96a19-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="96a19-109">Koble fra alle unødvendige enheter fra PC-en (for eksempel adaptere eller Docks).</span><span class="sxs-lookup"><span data-stu-id="96a19-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="96a19-110">**Hvis du nylig har installert en oppdatering på PC-en, kan du tilbakestille skjerm drive ren:**</span><span class="sxs-lookup"><span data-stu-id="96a19-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="96a19-111">Velg **Start**, Skriv inn **enhets behandling**, og velg **enhets behandling** fra resultatene.</span><span class="sxs-lookup"><span data-stu-id="96a19-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="96a19-112">Utvid **skjerm kort** delen, høyre klikk skjerm kortet, ands Velg **Egenskaper**.</span><span class="sxs-lookup"><span data-stu-id="96a19-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="96a19-113">Gå til **driver** -fanen, og velg **Rull driver tilbake**.</span><span class="sxs-lookup"><span data-stu-id="96a19-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="96a19-114">Obs! Hvis dette ikke er tilgjengelig eller er nedtonet, velger du **Nei** fra alternativene nedenfor for å gå til neste trinn.</span><span class="sxs-lookup"><span data-stu-id="96a19-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="96a19-115">Det kan hende du må starte PC-en på nytt før disse endringene trer i kraft.</span><span class="sxs-lookup"><span data-stu-id="96a19-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="96a19-116">**Avinstaller og Installer skjerm drive ren på nytt:**</span><span class="sxs-lookup"><span data-stu-id="96a19-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="96a19-117">Velg **Start**, Skriv inn **enhets behandling**, og velg **enhets behandling** fra resultatene.</span><span class="sxs-lookup"><span data-stu-id="96a19-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="96a19-118">Utvid **skjerm** kort delen, høyre klikk på skjerm kortet, ands Velg **Avinstaller enhet**.</span><span class="sxs-lookup"><span data-stu-id="96a19-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="96a19-119">Merk av i boksen ved siden av **Slett driver program varen for denne enheten** , og velg **Avinstaller**.</span><span class="sxs-lookup"><span data-stu-id="96a19-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="96a19-120">Obs! du kan bli bedt om å starte data maskinen på nytt på dette stadiet.</span><span class="sxs-lookup"><span data-stu-id="96a19-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="96a19-121">Pass på at du skriver ned de gjenværende instruksjonene før du starter på nytt.</span><span class="sxs-lookup"><span data-stu-id="96a19-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="96a19-122">Åpne enhets behandling på nytt.</span><span class="sxs-lookup"><span data-stu-id="96a19-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="96a19-123">Utvid **skjerm kort** delen, høyre klikk på skjerm kortet, og velg **Oppdater driver**.</span><span class="sxs-lookup"><span data-stu-id="96a19-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="96a19-124">Velg **Søk automatisk etter Oppdater driver program vare** og følg installasjons instruksjonene.</span><span class="sxs-lookup"><span data-stu-id="96a19-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>