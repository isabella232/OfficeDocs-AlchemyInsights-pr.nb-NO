---
title: Løse tilkoblingspolicy
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
- "9000760"
- "7391"
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695882"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="1d372-102">Løse tilkoblingspolicy</span><span class="sxs-lookup"><span data-stu-id="1d372-102">Fix connection policy</span></span>

<span data-ttu-id="1d372-103">E-postmeldingen ble merket som sikker og levert til brukerens innboks fordi ip-adressen som sendes, ble merket som sikker i policyen for tilkoblingsfilter.</span><span class="sxs-lookup"><span data-stu-id="1d372-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="1d372-104">Hvis du vil se gjennom policyen, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="1d372-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="1d372-105">Gå til sikkerhetssenteret [for Office 365 &,](https://go.microsoft.com/fwlink/p/?linkid=2077143)og gå deretter **til** beskyttelse mot søppelpost for  >    >  [trusselbehandling.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="1d372-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="1d372-106">Velg **policyen** for tilkoblingsfilter på Egendefinert-fanen, og velg deretter **Rediger policy.**</span><span class="sxs-lookup"><span data-stu-id="1d372-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="1d372-107">Se gjennom **ip-tillatelseslisten.**</span><span class="sxs-lookup"><span data-stu-id="1d372-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="1d372-108">Se om **klarerte lister** er aktivert.</span><span class="sxs-lookup"><span data-stu-id="1d372-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="1d372-109">Microsoft abonnerer på tredjepartskilder for klarerte avsendere.</span><span class="sxs-lookup"><span data-stu-id="1d372-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="1d372-110">Hvis **listen over klarerte** avsendere er aktivert, blir ikke disse klarerte avsenderne feilaktig merket som søppelpost.</span><span class="sxs-lookup"><span data-stu-id="1d372-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="1d372-111">Jeg anbefaler å velge dette alternativet fordi det vil redusere antall falske positiver (god e-post som klassifiseres som søppelpost) som du mottar.</span><span class="sxs-lookup"><span data-stu-id="1d372-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
