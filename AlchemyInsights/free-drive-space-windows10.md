---
title: Frigjøre diskplass i Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036591"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="773a4-102">Frigjøre diskplass i Windows 10</span><span class="sxs-lookup"><span data-stu-id="773a4-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="773a4-103">Her er to alternativer for å frigjøre diskplass i Windows:</span><span class="sxs-lookup"><span data-stu-id="773a4-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="773a4-104">Frigjør diskplass i Windows 10.</span><span class="sxs-lookup"><span data-stu-id="773a4-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="773a4-105">Frigjør plass til Windows 10-oppdateringer med ekstern lagringsenhet.</span><span class="sxs-lookup"><span data-stu-id="773a4-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="773a4-106">Hvis du fremdeles har lite diskplass etter å ha brukt Diskopprydding, er det mulig at Temp-mappen raskt fylles opp med programfiler (APPX) som brukes av Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="773a4-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="773a4-107">Hvis du vil løse dette problemet, tilbakestiller du Store, tømmer Store-bufferen og kjører deretter feilsøkingsprogrammet for Windows Update.</span><span class="sxs-lookup"><span data-stu-id="773a4-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="773a4-108">Kontroller at Microsoft Store er lukket før du fortsetter med disse trinnene.</span><span class="sxs-lookup"><span data-stu-id="773a4-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="773a4-109">**Trinn 1: Tilbakestille Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="773a4-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="773a4-110">**Obs!** Dette sletter appdataene på enheten permanent, inkludert innstillingene og påloggingsdetaljene.</span><span class="sxs-lookup"><span data-stu-id="773a4-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="773a4-111">Velg **Start**  >  **Innstillinger-apper**  >    >  **apper & funksjoner**.</span><span class="sxs-lookup"><span data-stu-id="773a4-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="773a4-112">Finn og velg Microsoft Store i listen over apper.</span><span class="sxs-lookup"><span data-stu-id="773a4-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="773a4-113">Velg **Avanserte alternativer**.</span><span class="sxs-lookup"><span data-stu-id="773a4-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="773a4-114">Rull nedover, **og velg Tilbakestill**, og deretter **Bekreft tilbakestilling**.</span><span class="sxs-lookup"><span data-stu-id="773a4-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="773a4-115">**Trinn 2: Tøm hurtigbufferen for Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="773a4-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="773a4-116">Trykk Windows-logotasten + R for å åpne dialogboksen Kjør.</span><span class="sxs-lookup"><span data-stu-id="773a4-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="773a4-117">Skriv wsreset.exe, og velg **OK**.</span><span class="sxs-lookup"><span data-stu-id="773a4-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="773a4-118">Et tomt ledetekstvindu åpnes.</span><span class="sxs-lookup"><span data-stu-id="773a4-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="773a4-119">Etter omtrent 10 sekunder lukkes vinduet, og Store åpnes automatisk.</span><span class="sxs-lookup"><span data-stu-id="773a4-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="773a4-120">**Trinn 3: Tilbakestille Windows Update**</span><span class="sxs-lookup"><span data-stu-id="773a4-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="773a4-121">Velg **Start innstillinger**  >  **Oppdater**&  >  **sikkerhetsfeilsøking**  >  .</span><span class="sxs-lookup"><span data-stu-id="773a4-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="773a4-122">Rull nedover og **velg Windows Update** fra listen, og velg Kjør **feilsøkingsprogrammet**.</span><span class="sxs-lookup"><span data-stu-id="773a4-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="773a4-123">Start datamaskinen på nytt, og kontroller om du fremdeles har problemet.</span><span class="sxs-lookup"><span data-stu-id="773a4-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

