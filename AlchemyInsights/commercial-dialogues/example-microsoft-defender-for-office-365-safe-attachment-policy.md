---
title: Eksempel på Microsoft Defender for policy for sikkert vedlegg i Office 365
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749202"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="045ae-102">Eksempel på Microsoft Defender for policy for sikkert vedlegg i Office 365</span><span class="sxs-lookup"><span data-stu-id="045ae-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="045ae-103">Disse innstillingene aktiverer en policy kalt *Ingen forsinkelser* som leverer meldinger umiddelbart, og deretter vedlegg på nytt etter at de er skannet:</span><span class="sxs-lookup"><span data-stu-id="045ae-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="045ae-104">**Navn:** Ingen forsinkelser</span><span class="sxs-lookup"><span data-stu-id="045ae-104">**Name**: No delays</span></span>
- <span data-ttu-id="045ae-105">**Beskrivelse:** Leverer meldinger umiddelbart, og vedlegg festes på nytt etter skanning.</span><span class="sxs-lookup"><span data-stu-id="045ae-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="045ae-106">**Svar:** Velg alternativet **Dynamisk** levering.</span><span class="sxs-lookup"><span data-stu-id="045ae-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="045ae-107">Hvis du vil ha mer informasjon, kan [du se Dynamisk levering i policyer for klarerte vedlegg](https://go.microsoft.com/fwlink/?linkid=2092328).</span><span class="sxs-lookup"><span data-stu-id="045ae-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="045ae-108">**Omdiriger** vedlegg-delen: Velg alternativet for å Aktivere omadressering **,** og skriv deretter inn e-postadressen til den globale microsoft 365-administratoren, sikkerhetsadministratoren eller sikkerhetsanalytikeren som skal undersøke skadelige vedlegg.</span><span class="sxs-lookup"><span data-stu-id="045ae-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="045ae-109">**Bruk på-delen:** **Velg Mottakerdomenet er**, og velg deretter domenet ditt.</span><span class="sxs-lookup"><span data-stu-id="045ae-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="045ae-110">Velg **Legg til**, og velg deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="045ae-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="045ae-111">Når du er ferdig, velger du **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="045ae-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="045ae-112">Hvis du vil ha mer informasjon, kan du [se Klarerte vedlegg i Microsoft Defender for Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)</span><span class="sxs-lookup"><span data-stu-id="045ae-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
