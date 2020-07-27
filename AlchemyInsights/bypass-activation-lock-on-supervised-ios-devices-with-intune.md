---
title: Omgå aktiveringslås på overvåkede iOS-enheter med Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424218"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="46332-102">Omgå aktiveringslås på overvåkede iOS-enheter med Intune</span><span class="sxs-lookup"><span data-stu-id="46332-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="46332-103">Muligheten til å omgå aktiveringslåsen på iOS-enheter gjør det enklere å gjenopprette fra scenariet der en bruker aktiverer aktiveringslås på en bedriftsenhet, og forlater deretter selskapet.</span><span class="sxs-lookup"><span data-stu-id="46332-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="46332-104">Forutsetninger for å omgå en aktiveringslås inkluderer:</span><span class="sxs-lookup"><span data-stu-id="46332-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="46332-105">En enhet er som er "overvåket".</span><span class="sxs-lookup"><span data-stu-id="46332-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="46332-106">Aktiveringslåsen er aktivert ved hjelp av policyen for begrensning av iOS-enhet i Intune.</span><span class="sxs-lookup"><span data-stu-id="46332-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="46332-107">I tillegg, når du omgår en aktiveringslås, bør du:</span><span class="sxs-lookup"><span data-stu-id="46332-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="46332-108">Fysisk besitte enheten blir tørket.</span><span class="sxs-lookup"><span data-stu-id="46332-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="46332-109">Kopier koden før du utsteder slettingen.</span><span class="sxs-lookup"><span data-stu-id="46332-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="46332-110">**Merk:** Tørkkoden skiller ikke mellom store og små bokstaver, så "-" tegnene er ikke nødvendig.</span><span class="sxs-lookup"><span data-stu-id="46332-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="46332-111">Hvis du vil ha mer informasjon, kan du se [Omgå aktiveringslås på overvåkede iOS-enheter med Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="46332-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="46332-112">**SPØRSMÅL OG SVAR**</span><span class="sxs-lookup"><span data-stu-id="46332-112">**FAQ**</span></span>

<span data-ttu-id="46332-113">Spørsmål: **Jeg utstedte en ekstern handling for å fjerne firmadata fra en enhet, og nå sitter det fast i en ventende tilstand.**</span><span class="sxs-lookup"><span data-stu-id="46332-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="46332-114">Svar: For at en ekstern handling skal kunne fullføres, må den målrettede enheten være tilkoblet og sunn.</span><span class="sxs-lookup"><span data-stu-id="46332-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="46332-115">I følgende situasjoner forblir den eksterne handlingen i ventende tilstand i 30 dager, eller til enheten erkjenner kommandoen når enheten:</span><span class="sxs-lookup"><span data-stu-id="46332-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="46332-116">Har ikke tilkobling.</span><span class="sxs-lookup"><span data-stu-id="46332-116">Does not have connectivity.</span></span>
- <span data-ttu-id="46332-117">Mister sin lederstatus med Intune.</span><span class="sxs-lookup"><span data-stu-id="46332-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="46332-118">Hvis du tror at en enhet ikke lenger sjekker inn, og at den ikke fjerner firmadata, velger du Slett.</span><span class="sxs-lookup"><span data-stu-id="46332-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="46332-119">Hvis du sletter enhetens post slik at den ikke lenger vises i Intune-listen over enheter.</span><span class="sxs-lookup"><span data-stu-id="46332-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="46332-120">For at enheten skal bli aktiv igjen, må brukeren registrere enheten på nytt.</span><span class="sxs-lookup"><span data-stu-id="46332-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="46332-121">Spørsmål: **Hvorfor er visse eksterne handlinger ikke tilgjengelige for meg å bruke?**</span><span class="sxs-lookup"><span data-stu-id="46332-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="46332-122">Svar: Ikke alle plattformer støtter alle handlinger for eksterne enheter.</span><span class="sxs-lookup"><span data-stu-id="46332-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="46332-123">Følgende eksterne handlinger er plattformspesifikke.</span><span class="sxs-lookup"><span data-stu-id="46332-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="46332-124">Bypass aktiveringslås (bare iOS)</span><span class="sxs-lookup"><span data-stu-id="46332-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="46332-125">Frisk start (bare Windows)</span><span class="sxs-lookup"><span data-stu-id="46332-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="46332-126">Tapt modus (bare iOS)</span><span class="sxs-lookup"><span data-stu-id="46332-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="46332-127">Finn enhet (bare iOS)</span><span class="sxs-lookup"><span data-stu-id="46332-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="46332-128">Start på nytt (bare Windows)</span><span class="sxs-lookup"><span data-stu-id="46332-128">Restart (Windows only)</span></span>

<span data-ttu-id="46332-129">Hvis du vil ha mer informasjon om hver handling, kan du se [Tilgjengelige enhetshandlinger](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="46332-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>