---
title: Sette planlagte oppdateringer på pause
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555513"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="0014f-102">Sette planlagte oppdateringer på pause</span><span class="sxs-lookup"><span data-stu-id="0014f-102">Pausing scheduled updates</span></span>

<span data-ttu-id="0014f-103">Når en pause-kommando utstedes, behandler ikke enheter kommandoen før neste gang de sjekker inn på Intune.</span><span class="sxs-lookup"><span data-stu-id="0014f-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="0014f-104">På grunn av dette kan enhetene dine ha:</span><span class="sxs-lookup"><span data-stu-id="0014f-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="0014f-105">Installert de planlagte oppdateringene før innsjekking.</span><span class="sxs-lookup"><span data-stu-id="0014f-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="0014f-106">Blitt slått av da du utstedte pausekommandoen.</span><span class="sxs-lookup"><span data-stu-id="0014f-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="0014f-107">I dette tilfellet, når enhetene ble slått på, kan de ha lastet ned og installert de planlagte oppdateringene før innsjekking.</span><span class="sxs-lookup"><span data-stu-id="0014f-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>