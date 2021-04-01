---
title: Angi Microsoft Edge som standard nettleser på en MacOS-enhet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491809"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="92267-102">Angi Microsoft Edge som standard nettleser på en MacOS-enhet</span><span class="sxs-lookup"><span data-stu-id="92267-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="92267-103">Bruk én av disse to metodene til å angi Microsoft Edge som standardleser:</span><span class="sxs-lookup"><span data-stu-id="92267-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="92267-104">Metode 1: Blink enheten med et bilde av macOS der Microsoft Edge allerede er angitt som standard nettleser.</span><span class="sxs-lookup"><span data-stu-id="92267-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="92267-105">Metode 2: Angi DefaultBrowserSettingEnabled-policyen for å be brukeren om å angi Microsoft Edge som standardleser.</span><span class="sxs-lookup"><span data-stu-id="92267-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="92267-106">Med begge metodene kan en bruker endre standardleseren.</span><span class="sxs-lookup"><span data-stu-id="92267-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="92267-107">Derfor anbefaler vi at du distribuerer DefaultBrowserSettingEnabled-policyen selv om du brukte metode 1.</span><span class="sxs-lookup"><span data-stu-id="92267-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="92267-108">Hvis en bruker endrer standardleseren etter at policyen er distribuert, blir brukeren bedt om å angi standardleseren tilbake til Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="92267-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
