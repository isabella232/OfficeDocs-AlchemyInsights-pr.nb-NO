---
title: Løse tenantpolicy (handlingsoverstyring)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748994"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="e0270-102">Løse tenantpolicy (handlingsoverstyring)</span><span class="sxs-lookup"><span data-stu-id="e0270-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="e0270-103">En policy for søppelpost i tenanten påvirket denne meldingen.</span><span class="sxs-lookup"><span data-stu-id="e0270-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="e0270-104">Gjør følgende for å se gjennom policyen:</span><span class="sxs-lookup"><span data-stu-id="e0270-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="e0270-105">Gå til sikkerhets- og samsvarssenteret [for Office 365 &](https://go.microsoft.com/fwlink/p/?linkid=2077143), og gå deretter til Policy for beskyttelse mot søppelpost for   >    >  [trusler.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="e0270-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="e0270-106">Kontroller om **Policykilde** angir følgende:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ Blindkopi-melding**</span><span class="sxs-lookup"><span data-stu-id="e0270-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="e0270-107">Hvis dette er det, **kontrollerer** du innstillingene for policyen som påvirket meldingen, på Egendefinert-fanen.</span><span class="sxs-lookup"><span data-stu-id="e0270-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="e0270-108">Det er mulig at **standardinnstillingene som** ble brukt på alle Exchange Online Protection-kunder, påvirket meldingen.</span><span class="sxs-lookup"><span data-stu-id="e0270-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="e0270-109">Hvis du vil ha mer informasjon om hvordan du konfigurerer policyer for søppelpostfilter, kan [du se Konfigurere policyer for søppelpostfilter .](https://go.microsoft.com/fwlink/?linkid=2101431)</span><span class="sxs-lookup"><span data-stu-id="e0270-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
