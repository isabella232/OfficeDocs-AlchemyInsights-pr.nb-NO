---
title: Feilsøke eksisterende skjerm
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738577"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="a153e-102">Feilsøk en eksisterende skjerm</span><span class="sxs-lookup"><span data-stu-id="a153e-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="a153e-103">Prøv disse løsningene for å feilsøke en skjerm.</span><span class="sxs-lookup"><span data-stu-id="a153e-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="a153e-104">**Oppdater skjermens skjerm:**</span><span class="sxs-lookup"><span data-stu-id="a153e-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="a153e-105">Trykk på følgende taster samtidig: Windows-tast + Ctrl + Shift + B. Dette vil oppdatere kommunikasjonen med grafikkdriveren din.</span><span class="sxs-lookup"><span data-stu-id="a153e-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="a153e-106">Skjermene vil blinke et øyeblikk og komme tilbake etter noen sekunder.</span><span class="sxs-lookup"><span data-stu-id="a153e-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="a153e-107">**Feilsøke skjermmaskinvare:**</span><span class="sxs-lookup"><span data-stu-id="a153e-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="a153e-108">Koble fra kabelen som kobler PCen til skjermen, og koble den til på nytt.</span><span class="sxs-lookup"><span data-stu-id="a153e-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="a153e-109">Koble fra alle ikke-essensielle enheter fra PC-en (for eksempel adaptere eller dokkingstasjoner).</span><span class="sxs-lookup"><span data-stu-id="a153e-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="a153e-110">**Hvis du nylig har installert en oppdatering på PC-en, kan du rulle tilbake skjermdriveren:**</span><span class="sxs-lookup"><span data-stu-id="a153e-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="a153e-111">Velg **Start**, Skriv inn **Enhetsbehandling**, og velg **Enhetsbehandling** fra resultatene.</span><span class="sxs-lookup"><span data-stu-id="a153e-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="a153e-112">Utvid delen **skjermkort** , høyreklikk skjermkortet, ands Velg **Egenskaper**.</span><span class="sxs-lookup"><span data-stu-id="a153e-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="a153e-113">Naviger til **driver** fanen og velg **Rull tilbake driver**.</span><span class="sxs-lookup"><span data-stu-id="a153e-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="a153e-114">Merk: Hvis dette ikke er tilgjengelig eller er nedtonet, velger du **Nei** fra alternativene nedenfor for å gå til neste trinn.</span><span class="sxs-lookup"><span data-stu-id="a153e-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="a153e-115">Du må kanskje starte PC-en på nytt før disse endringene trer i kraft.</span><span class="sxs-lookup"><span data-stu-id="a153e-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="a153e-116">**Avinstaller skjermdriveren og Installer den på nytt:**</span><span class="sxs-lookup"><span data-stu-id="a153e-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="a153e-117">Velg **Start**, Skriv inn **Enhetsbehandling**, og velg **Enhetsbehandling** fra resultatene.</span><span class="sxs-lookup"><span data-stu-id="a153e-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="a153e-118">Utvid delen **skjermkort** , høyreklikk skjermkortet, ands Velg **Avinstaller enhet**.</span><span class="sxs-lookup"><span data-stu-id="a153e-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="a153e-119">Merk av i boksen ved siden av **Slett driverprogramvaren for denne enheten** , og velg **Avinstaller**.</span><span class="sxs-lookup"><span data-stu-id="a153e-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="a153e-120">Merk: du kan bli bedt om å starte datamaskinen på nytt på dette stadiet.</span><span class="sxs-lookup"><span data-stu-id="a153e-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="a153e-121">Husk å skrive ned resten av instruksjonene før du starter på nytt.</span><span class="sxs-lookup"><span data-stu-id="a153e-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="a153e-122">Åpne Enhetsbehandling på nytt.</span><span class="sxs-lookup"><span data-stu-id="a153e-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="a153e-123">Utvid delen **skjermkort** , høyreklikk skjermkortet, og velg **Oppdater driver**.</span><span class="sxs-lookup"><span data-stu-id="a153e-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="a153e-124">Velg **Søk automatisk for å oppdatere driverprogramvare** og følg installeringsinstruksjonene.</span><span class="sxs-lookup"><span data-stu-id="a153e-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>