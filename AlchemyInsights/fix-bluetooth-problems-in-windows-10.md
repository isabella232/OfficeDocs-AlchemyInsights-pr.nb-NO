---
title: Løse problemer med Bluetooth i Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730168"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="5dc5f-102">Løse problemer med Bluetooth i Windows 10</span><span class="sxs-lookup"><span data-stu-id="5dc5f-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="5dc5f-103">Hvis Bluetooth-ikonet mangler eller Bluetooth ikke kan slås på eller av, vil du kanskje kjøre Bluetooth-feilsøking.</span><span class="sxs-lookup"><span data-stu-id="5dc5f-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="5dc5f-104">[Åpne feil søkings innstillinger](ms-settings:troubleshoot), klikk på **Bluetooth** under **Finn og løs andre problemer**, og klikk **Kjør feil søking**.</span><span class="sxs-lookup"><span data-stu-id="5dc5f-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="5dc5f-105">Hvis du ikke ser Bluetooth-ikonet, men Bluetooth vises i enhets behandling:</span><span class="sxs-lookup"><span data-stu-id="5dc5f-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="5dc5f-106">Klikk **Bluetooth**i enhets behandling.</span><span class="sxs-lookup"><span data-stu-id="5dc5f-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="5dc5f-107">Trykk og hold (eller høyre klikk) navnet på Bluetooth-kortet, og klikk **Avinstaller enhet**.</span><span class="sxs-lookup"><span data-stu-id="5dc5f-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="5dc5f-108">Avslutt Windows-enheten, vent noen sekunder, og slå den deretter på igjen.</span><span class="sxs-lookup"><span data-stu-id="5dc5f-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="5dc5f-109">Windows vil prøve å installere driveren på nytt.</span><span class="sxs-lookup"><span data-stu-id="5dc5f-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="5dc5f-110">Hvis du nylig har installert Windows 10-oppdateringer eller oppgradert til Windows 10, kan det hende du vil se etter driver oppdateringer:</span><span class="sxs-lookup"><span data-stu-id="5dc5f-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="5dc5f-111">Klikk **Bluetooth**i enhets behandling, og klikk deretter navnet på Bluetooth-kortet (som kan inneholde ordet radio).</span><span class="sxs-lookup"><span data-stu-id="5dc5f-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="5dc5f-112">Trykk og hold (eller høyre klikk) Bluetooth-adapteren, og klikk deretter **Oppdater driver**  >  **Søk automatisk for oppdatert driver program vare**.</span><span class="sxs-lookup"><span data-stu-id="5dc5f-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="5dc5f-113">Følg trinnene, og klikk deretter **Lukk**.</span><span class="sxs-lookup"><span data-stu-id="5dc5f-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="5dc5f-114">Hvis Windows ikke finner en ny Bluetooth-driver, kan du gå til PC-produsentens nettsted og laste ned den nyeste Bluetooth-driveren derfra.</span><span class="sxs-lookup"><span data-stu-id="5dc5f-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="5dc5f-115">Når du har lastet den ned, klikker du **Oppdater driver**  >  **Bla gjennom data maskinen etter driver program vare**  >  **Bla gjennom** for plasseringen der driver filene er lagret > **OK**  >  **neste**, og følg trinnene for å installere.</span><span class="sxs-lookup"><span data-stu-id="5dc5f-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="5dc5f-116">Når du har installert den oppdaterte driveren, starter du data maskinen på nytt, og deretter kontrollerer du om det løser tilkoblings problemet.</span><span class="sxs-lookup"><span data-stu-id="5dc5f-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="5dc5f-117">Hvis du vil ha mer informasjon om hvordan du feil søker Bluetooth-problemer, kan du se den fullstendige artikkelen, [løse problemer med Bluetooth i Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="5dc5f-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
