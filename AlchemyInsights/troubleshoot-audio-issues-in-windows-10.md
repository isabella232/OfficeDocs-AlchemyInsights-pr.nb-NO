---
title: Feilsøke lydproblemer i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 46b23f97c2e682258224dc95e7a76b1201991828
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796267"
---
# <a name="troubleshooting-audio-problems-in-windows-10"></a><span data-ttu-id="577b2-102">Feilsøke lydproblemer i Windows 10</span><span class="sxs-lookup"><span data-stu-id="577b2-102">Troubleshooting audio problems in Windows 10</span></span>

<span data-ttu-id="577b2-103">**Kjøre feilsøking for lyd**</span><span class="sxs-lookup"><span data-stu-id="577b2-103">**Run the audio troubleshooter**</span></span>

<span data-ttu-id="577b2-104">Feilsøking for lyd kan være i stand til å løse lyd problemene automatisk:</span><span class="sxs-lookup"><span data-stu-id="577b2-104">The audio troubleshooter might be able to fix the audio problems automatically:</span></span> 

1. <span data-ttu-id="577b2-105">Velg **Start**, Skriv **feilsøking**, og velg deretter **Feilsøk** fra listen over resultater.</span><span class="sxs-lookup"><span data-stu-id="577b2-105">Select **Start**, type **troubleshoot**, and then select **Troubleshoot** from the list of results.</span></span> 
2. <span data-ttu-id="577b2-106">Velg **å spille av lyd** > **Kjør feilsøkingsprogrammet**.</span><span class="sxs-lookup"><span data-stu-id="577b2-106">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="577b2-107">**Kontroller kabler, volum, høyttalere og hodetelefoner**</span><span class="sxs-lookup"><span data-stu-id="577b2-107">**Check cables, volume, speakers, and headphones**</span></span>

- <span data-ttu-id="577b2-108">Kontroller tilkoblingene til høyttalerne og hodetelefonene for løse kabler, og kontroller at de er koblet til riktig kontakt.</span><span class="sxs-lookup"><span data-stu-id="577b2-108">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>
- <span data-ttu-id="577b2-109">Kontroller strøm-og volumnivået, og prøv å slå alle volumkontrollene opp.</span><span class="sxs-lookup"><span data-stu-id="577b2-109">Check your power and volume levels, and try turning all the volume controls up.</span></span>
- <span data-ttu-id="577b2-110">Noen høyttalere og apper har egne volumkontroller, og du må kanskje kontrollere dem for å sikre at de er på riktig nivå.</span><span class="sxs-lookup"><span data-stu-id="577b2-110">Some speakers and apps have their own volume controls, and you might have to check them all to make sure they're at the right levels.</span></span>
- <span data-ttu-id="577b2-111">Prøv å koble til med en annen USB-port.</span><span class="sxs-lookup"><span data-stu-id="577b2-111">Try connecting using a different USB port.</span></span>
- <span data-ttu-id="577b2-112">**Merk:** Husk at høyttalerne kanskje ikke fungerer når hodetelefonene er plugget inn.</span><span class="sxs-lookup"><span data-stu-id="577b2-112">**Note:** Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="577b2-113">**Kontroller Enhetsbehandling**</span><span class="sxs-lookup"><span data-stu-id="577b2-113">**Check Device Manager**</span></span>

<span data-ttu-id="577b2-114">Slik kontrollerer du at driverne er oppdatert:</span><span class="sxs-lookup"><span data-stu-id="577b2-114">To make sure the drivers are up to date:</span></span>

- <span data-ttu-id="577b2-115">Velg **Start**, Skriv inn **Enhetsbehandling**, og velg deretter **Enhetsbehandling** fra listen over resultater.</span><span class="sxs-lookup"><span data-stu-id="577b2-115">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="577b2-116">Under **lyd-, video-og spillkontrollere**velger du lydkortet, åpner det, velger **driver** -fanen og velger **Oppdater driver**.</span><span class="sxs-lookup"><span data-stu-id="577b2-116">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span> 

<span data-ttu-id="577b2-117">**Merk:** Hvis Windows ikke finner en ny driver, kan du se etter en på enhetsprodusentens webområde og følge instruksjonene deres.</span><span class="sxs-lookup"><span data-stu-id="577b2-117">**Note:** If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="577b2-118">**Installer driveren på nytt**</span><span class="sxs-lookup"><span data-stu-id="577b2-118">**Reinstall the driver**</span></span>

<span data-ttu-id="577b2-119">Hvis du ikke kan oppdatere via Enhetsbehandling eller finne en ny driver på produsentens webområde, kan du prøve disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="577b2-119">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span> 

1. <span data-ttu-id="577b2-120">I Enhetsbehandling høyreklikker du (eller trykker og holder) lyddriveren, og velger **Avinstaller**.</span><span class="sxs-lookup"><span data-stu-id="577b2-120">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="577b2-121">Start enheten på nytt, og Windows prøver å installere driveren på nytt.</span><span class="sxs-lookup"><span data-stu-id="577b2-121">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="577b2-122">Hvis det ikke fungerer å installere driveren på nytt, kan du prøve å bruke den generiske lyddriveren som følger med Windows.</span><span class="sxs-lookup"><span data-stu-id="577b2-122">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="577b2-123">I Enhetsbehandling høyreklikker du (eller trykker og holder) lyddriveren > **oppdatere driverprogramvare** > **Søk på datamaskinen etter driverprogramvare** > **La meg velge fra en liste over enhetsdrivere på datamaskinen**, velge **High Definition Audio-enhet**, velge **neste**og følge instruksjonene for å installere den.</span><span class="sxs-lookup"><span data-stu-id="577b2-123">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>

<span data-ttu-id="577b2-124">**Angi standard enhet**</span><span class="sxs-lookup"><span data-stu-id="577b2-124">**Set the default device**</span></span>

<span data-ttu-id="577b2-125">Hvis du kobler til en lydenhet ved hjelp av USB eller HDMI, må du kanskje angi denne enheten som standard:</span><span class="sxs-lookup"><span data-stu-id="577b2-125">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span> 

1. <span data-ttu-id="577b2-126">Velg **Start**, Skriv inn **lyd**, og velg deretter **lyd** eller **endre system lyder** fra resultatlisten.</span><span class="sxs-lookup"><span data-stu-id="577b2-126">Select **Start**, type **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2. <span data-ttu-id="577b2-127">Velg en enhet i kategorien **avspilling** , velg **Angi standard**, og velg deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="577b2-127">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

