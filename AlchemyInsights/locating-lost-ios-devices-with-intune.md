---
title: Finne tapte iOS-enheter med Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440435"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="0cfe8-102">Finne tapte iOS-enheter med Intune</span><span class="sxs-lookup"><span data-stu-id="0cfe8-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="0cfe8-103">Aktivering av tapt modus på en iOS-enhet gjør det mulig for en administrator å få en melding og kontakttelefonnummer vist på låseskjermen.</span><span class="sxs-lookup"><span data-stu-id="0cfe8-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="0cfe8-104">Når tapt modus er aktivert, kan administratoren bruke handlingen Finn enhet til å identifisere enhetens fysiske plassering.</span><span class="sxs-lookup"><span data-stu-id="0cfe8-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="0cfe8-105">Handlingen Finn enhet i Intune fungerer med iOS-enheter for å vise plasseringen av en bestemt enhet på et kart.</span><span class="sxs-lookup"><span data-stu-id="0cfe8-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="0cfe8-106">Bruk av denne handlingen krever at iOS-enheten er i:</span><span class="sxs-lookup"><span data-stu-id="0cfe8-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="0cfe8-107">Overvåket modus</span><span class="sxs-lookup"><span data-stu-id="0cfe8-107">Supervised mode</span></span>
- <span data-ttu-id="0cfe8-108">Tapt modus</span><span class="sxs-lookup"><span data-stu-id="0cfe8-108">Lost mode</span></span>

<span data-ttu-id="0cfe8-109">Hvis du vil ha mer informasjon, kan du se [Aktivere tapt modus på iOS/iPadOS-enheter med Intune](https://docs.microsoft.com/intune/device-lost-mode) og Finn tapte eller [stjålne iOS/iPadOS-enheter med Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="0cfe8-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="0cfe8-110">**SPØRSMÅL OG SVAR**</span><span class="sxs-lookup"><span data-stu-id="0cfe8-110">**FAQ**</span></span>

<span data-ttu-id="0cfe8-111">Spørsmål: Jeg utstedte en ekstern handling for å fjerne firmadata fra en enhet, og nå sitter det fast i en ventende tilstand.</span><span class="sxs-lookup"><span data-stu-id="0cfe8-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="0cfe8-112">Svar: For at en ekstern handling skal kunne fullføres, må den målrettede enheten være tilkoblet og sunn.</span><span class="sxs-lookup"><span data-stu-id="0cfe8-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="0cfe8-113">I følgende situasjoner forblir den eksterne handlingen i ventende tilstand i 30 dager, eller til enheten erkjenner kommandoen:</span><span class="sxs-lookup"><span data-stu-id="0cfe8-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="0cfe8-114">Når enheten ikke har tilkobling</span><span class="sxs-lookup"><span data-stu-id="0cfe8-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="0cfe8-115">Når enheten mister administrasjonsstatusen med Intune</span><span class="sxs-lookup"><span data-stu-id="0cfe8-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="0cfe8-116">Hvis du tror at en enhet ikke lenger sjekker inn, og at den ikke kan fjerne firmadata, velger du Slett.</span><span class="sxs-lookup"><span data-stu-id="0cfe8-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="0cfe8-117">Hvis du sletter enhetens post slik at den ikke lenger vises i Intune-listen over enheter.</span><span class="sxs-lookup"><span data-stu-id="0cfe8-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="0cfe8-118">Hvis enheten blir aktiv igjen, må brukeren registrere den på nytt.</span><span class="sxs-lookup"><span data-stu-id="0cfe8-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="0cfe8-119">Spørsmål: Hvorfor er visse eksterne handlinger ikke tilgjengelige for meg å bruke?</span><span class="sxs-lookup"><span data-stu-id="0cfe8-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="0cfe8-120">Svar: Ikke alle plattformer støtter alle handlinger for eksterne enheter.</span><span class="sxs-lookup"><span data-stu-id="0cfe8-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="0cfe8-121">Følgende eksterne handlinger er plattformspesifikke, så de er bare tilgjengelige for plattformene som er nevnt.</span><span class="sxs-lookup"><span data-stu-id="0cfe8-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="0cfe8-122">Bypass aktiveringslås (bare iOS)</span><span class="sxs-lookup"><span data-stu-id="0cfe8-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="0cfe8-123">Frisk start (bare Windows)</span><span class="sxs-lookup"><span data-stu-id="0cfe8-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="0cfe8-124">Tapt modus (bare iOS)</span><span class="sxs-lookup"><span data-stu-id="0cfe8-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="0cfe8-125">Finn enhet (bare iOS)</span><span class="sxs-lookup"><span data-stu-id="0cfe8-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="0cfe8-126">Start på nytt (bare Windows)</span><span class="sxs-lookup"><span data-stu-id="0cfe8-126">Restart (Windows only)</span></span>

<span data-ttu-id="0cfe8-127">Hvis du vil ha mer informasjon om hver handling, kan du se [Tilgjengelige enhetshandlinger](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="0cfe8-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>