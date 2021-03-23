---
title: Hindre at meldinger flyttes til arkivet automatisk
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749826"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="825ee-102">Hindre at meldinger flyttes til arkivet automatisk</span><span class="sxs-lookup"><span data-stu-id="825ee-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="825ee-103">Hvis du bruker en oppbevaringspolicy, kan du endre oppbevaringsalderen i denne policyen for å hindre at meldinger arkiveres automatisk.</span><span class="sxs-lookup"><span data-stu-id="825ee-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="825ee-104">Slik gjør du det:</span><span class="sxs-lookup"><span data-stu-id="825ee-104">Here's how:</span></span>

1. <span data-ttu-id="825ee-105">Velg [oppbevaringskoder for](https://go.microsoft.com/fwlink/?linkid=2059104) **samsvarsbehandling** i administrasjonssenteret  >  **for** Exchange.</span><span class="sxs-lookup"><span data-stu-id="825ee-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="825ee-106">Finn oppbevaringskoden Flytt til arkiv.</span><span class="sxs-lookup"><span data-stu-id="825ee-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="825ee-107">I oppbevaringskoden endrer du oppbevaringsperioden  (arkivperioden) til Aldri for å hindre at elementer arkiveres automatisk av en oppbevaringspolicy.</span><span class="sxs-lookup"><span data-stu-id="825ee-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="825ee-108">Dette endrer arkivinnstillingen for alle postbokser med denne oppbevaringskoden brukt på dem.</span><span class="sxs-lookup"><span data-stu-id="825ee-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>