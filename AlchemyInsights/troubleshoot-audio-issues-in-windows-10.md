---
title: Feilsøke lydproblemer i Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833300"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="885d3-102">Feilsøke lydproblemer i Windows 10</span><span class="sxs-lookup"><span data-stu-id="885d3-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="885d3-103">**Kjøre feilsøking for lyd**</span><span class="sxs-lookup"><span data-stu-id="885d3-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="885d3-104">Åpne [feilsøkingsinnstillingene](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="885d3-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="885d3-105">Velg **Spill av lyd** Kjør  >  **feilsøkingsprogrammet**.</span><span class="sxs-lookup"><span data-stu-id="885d3-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="885d3-106">**Angi standardenheten**</span><span class="sxs-lookup"><span data-stu-id="885d3-106">**Set the default device**</span></span>

<span data-ttu-id="885d3-107">Hvis du kobler til en lydenhet ved hjelp av USB eller HDMI, må du kanskje angi denne enheten som standard:</span><span class="sxs-lookup"><span data-stu-id="885d3-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="885d3-108">Åpne **Start**  >  **lyd**, og velg deretter **Lyd** eller **Endre systemlyder** fra listen over resultater.</span><span class="sxs-lookup"><span data-stu-id="885d3-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="885d3-109">Velg en **enhet** på Avspilling-fanen, velg **Angi standard**, og velg deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="885d3-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="885d3-110">**Kontroller kabler, volum, høyttalere og hodetelefoner**</span><span class="sxs-lookup"><span data-stu-id="885d3-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="885d3-111">Kontroller høyttaler- og hodetelefontilkoblingene for løse kabler, og kontroller at de er koblet til riktig kontakt.</span><span class="sxs-lookup"><span data-stu-id="885d3-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="885d3-112">Kontroller strøm- og volumnivåene, og prøv å skru opp alle volumkontrollene.</span><span class="sxs-lookup"><span data-stu-id="885d3-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="885d3-113">Noen høyttalere og apper har sine egne volumkontroller. Du må kanskje kontrollere alle for å sikre at de er på riktig nivå.</span><span class="sxs-lookup"><span data-stu-id="885d3-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="885d3-114">Prøv å koble til med en annen USB-port.</span><span class="sxs-lookup"><span data-stu-id="885d3-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="885d3-115">**Obs!** Husk at høyttalerne kanskje ikke fungerer når hodetelefonene er koblet til.</span><span class="sxs-lookup"><span data-stu-id="885d3-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="885d3-116">**Kontroller Enhetsbehandling**</span><span class="sxs-lookup"><span data-stu-id="885d3-116">**Check Device Manager**</span></span>

<span data-ttu-id="885d3-117">Slik kontrollerer du at driverne er oppdatert:</span><span class="sxs-lookup"><span data-stu-id="885d3-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="885d3-118">Velg **Start**, skriv **inn Enhetsbehandling**, og velg deretter **Enhetsbehandling** fra listen over resultater.</span><span class="sxs-lookup"><span data-stu-id="885d3-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="885d3-119">Velg **lydkortet under Lyd-, video-** og spillkontrollere, åpne det, velg **Driver-fanen** og velg **Oppdater driver**.</span><span class="sxs-lookup"><span data-stu-id="885d3-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="885d3-120">**Obs!** Hvis Windows ikke finner en ny driver, kan du se etter en på nettstedet til enhetsprodusenten og følge instruksjonene deres.</span><span class="sxs-lookup"><span data-stu-id="885d3-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="885d3-121">**Installere driveren på nytt**</span><span class="sxs-lookup"><span data-stu-id="885d3-121">**Reinstall the driver**</span></span>

<span data-ttu-id="885d3-122">Hvis du ikke kan oppdatere via Enhetsbehandling eller finne en ny driver på produsentens nettsted, kan du prøve disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="885d3-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="885d3-123">Høyreklikk (eller trykk og hold) lyddriveren i **Enhetsbehandling,** og velg Avinstaller .</span><span class="sxs-lookup"><span data-stu-id="885d3-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="885d3-124">Start enheten på nytt, så prøver Windows å installere driveren på nytt.</span><span class="sxs-lookup"><span data-stu-id="885d3-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="885d3-125">Hvis det ikke fungerer å installere driveren på nytt, kan du prøve å bruke den generiske lyddriveren som følger med Windows.</span><span class="sxs-lookup"><span data-stu-id="885d3-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="885d3-126">Høyreklikk (eller trykk og hold) lyddriveren i Enhetsbehandling > Oppdater driverprogramvaren Bla gjennom datamaskinen for driverprogramvaren La meg velge fra en liste over enhetsdrivere på datamaskinen, velg  >    >    **Hd-lydenhet,** velg Neste , og følg instruksjonene for å installere den.</span><span class="sxs-lookup"><span data-stu-id="885d3-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
