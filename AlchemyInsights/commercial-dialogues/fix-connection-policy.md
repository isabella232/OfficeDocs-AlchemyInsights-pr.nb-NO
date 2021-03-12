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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750606"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="7c5de-102">Løse tilkoblingspolicy</span><span class="sxs-lookup"><span data-stu-id="7c5de-102">Fix connection policy</span></span>

<span data-ttu-id="7c5de-103">E-postmeldingen ble merket som sikker og levert til brukerens innboks fordi den sendte IP-adressen ble merket som sikker i policyen for tilkoblingsfilteret.</span><span class="sxs-lookup"><span data-stu-id="7c5de-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="7c5de-104">Gjør følgende for å se gjennom policyen:</span><span class="sxs-lookup"><span data-stu-id="7c5de-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="7c5de-105">Gå til sikkerhets- og samsvarssenteret [for Office 365 &](https://go.microsoft.com/fwlink/p/?linkid=2077143), og gå deretter til Policy for beskyttelse mot søppelpost for   >    >  [trusler.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="7c5de-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="7c5de-106">Velg Policy **for** tilkoblingsfilter på Egendefinert-fanen, og velg deretter Rediger **policy**.</span><span class="sxs-lookup"><span data-stu-id="7c5de-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="7c5de-107">Se gjennom **tillatelseslisten for IP.**</span><span class="sxs-lookup"><span data-stu-id="7c5de-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="7c5de-108">Se om **Sikker-listen** er aktivert.</span><span class="sxs-lookup"><span data-stu-id="7c5de-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="7c5de-109">Microsoft abonnerer på tredjepartskilder for klarerte avsendere.</span><span class="sxs-lookup"><span data-stu-id="7c5de-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="7c5de-110">Hvis **Sikker-listen** er aktivert, merkes ikke disse klarerte avsenderne feilaktig som søppelpost.</span><span class="sxs-lookup"><span data-stu-id="7c5de-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="7c5de-111">Jeg anbefaler å velge dette alternativet, fordi det vil redusere antall falske positiver (god e-post som er klassifisert som søppelpost) som du mottar.</span><span class="sxs-lookup"><span data-stu-id="7c5de-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
