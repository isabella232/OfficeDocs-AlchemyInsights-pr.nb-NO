---
title: Frigjør diskplass i Windows 10
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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505365"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="4aa79-102">Frigjør diskplass i Windows 10</span><span class="sxs-lookup"><span data-stu-id="4aa79-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="4aa79-103">Her er to alternativer for å frigjøre diskplass i Windows:</span><span class="sxs-lookup"><span data-stu-id="4aa79-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="4aa79-104">Frigjøre diskplass i Windows 10.</span><span class="sxs-lookup"><span data-stu-id="4aa79-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="4aa79-105">Frigjør plass for oppdateringer for Windows 10 med ekstern lagringsenhet.</span><span class="sxs-lookup"><span data-stu-id="4aa79-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="4aa79-106">Hvis du fremdeles har lite diskplass etter å ha brukt Diskopprydding, er det mulig at den midlertidige mappen raskt fylles opp med programfiler (.appx) som brukes av Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="4aa79-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="4aa79-107">Du kan løse dette problemet ved å tilbakestille Store, tømme hurtigbufferen for Store og deretter kjøre feilsøkingsverktøyet for Windows Update.</span><span class="sxs-lookup"><span data-stu-id="4aa79-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="4aa79-108">Kontroller at Microsoft Store er lukket før du fortsetter med disse trinnene.</span><span class="sxs-lookup"><span data-stu-id="4aa79-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="4aa79-109">**Trinn 1: Tilbakestill Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="4aa79-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="4aa79-110">**Obs!** Dette sletter app-dataene på enheten permanent, inkludert preferanser og påloggingsdetaljer.</span><span class="sxs-lookup"><span data-stu-id="4aa79-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="4aa79-111">Velg **Start** > **innstillinger** > **Apper** > **Apper og funksjoner**.</span><span class="sxs-lookup"><span data-stu-id="4aa79-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="4aa79-112">Finn og velg Microsoft Store i listen over apper.</span><span class="sxs-lookup"><span data-stu-id="4aa79-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="4aa79-113">Velg **Avanserte alternativer**.</span><span class="sxs-lookup"><span data-stu-id="4aa79-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="4aa79-114">Rull nedover og velg **Tilbakestill**, og deretter **Bekreft tilbakestilling**.</span><span class="sxs-lookup"><span data-stu-id="4aa79-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="4aa79-115">**Trinn 2: Tøm bufferen for Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="4aa79-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="4aa79-116">Trykk Windows-tasten + R for å åpne dialogboksen Kjør.</span><span class="sxs-lookup"><span data-stu-id="4aa79-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="4aa79-117">Skriv inn wsreset.exe, og **OK**.</span><span class="sxs-lookup"><span data-stu-id="4aa79-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="4aa79-118">Et tomt ledetekstvindu åpnes.</span><span class="sxs-lookup"><span data-stu-id="4aa79-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="4aa79-119">Etter omtrent 10 sekunder lukkes vinduet, og Store åpnes automatisk.</span><span class="sxs-lookup"><span data-stu-id="4aa79-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="4aa79-120">**Trinn 3: Tilbakestill Windows Update**</span><span class="sxs-lookup"><span data-stu-id="4aa79-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="4aa79-121">Velg **Start** > **Innstillinger** > **Oppdatering og sikkerhet** > **Feilsøk**.</span><span class="sxs-lookup"><span data-stu-id="4aa79-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="4aa79-122">Rull nedover og velg **Windows Update** fra listen, og velg **Kjør feilsøkingsverktøyet**.</span><span class="sxs-lookup"><span data-stu-id="4aa79-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="4aa79-123">Start datamaskinen på nytt, og kontroller om du fremdeles har dette problemet.</span><span class="sxs-lookup"><span data-stu-id="4aa79-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

