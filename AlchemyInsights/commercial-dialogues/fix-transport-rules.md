---
title: Løse transportregler
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750580"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="dd02e-102">Løse transportregler</span><span class="sxs-lookup"><span data-stu-id="dd02e-102">Fix transport rules</span></span>

<span data-ttu-id="dd02e-103">En egendefinert e-postflytregel påvirket denne meldingen.</span><span class="sxs-lookup"><span data-stu-id="dd02e-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="dd02e-104">Hvis du vil se gjennom den nøyaktige regelen, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="dd02e-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="dd02e-105">Legg merke til GUID-en eller  policynavnet under **Tilleggsinformasjon** i **innsendingsresultatene.**</span><span class="sxs-lookup"><span data-stu-id="dd02e-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="dd02e-106">Start Skallet for Exchange-administrasjon.</span><span class="sxs-lookup"><span data-stu-id="dd02e-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="dd02e-107">Hvis du vil ha mer informasjon, [kan du se Åpne Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="dd02e-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="dd02e-108">Kjør denne kommandoen (ved hjelp av GUID fra innsendingen):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span><span class="sxs-lookup"><span data-stu-id="dd02e-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="dd02e-109">Se gjennom beskrivelsen for å se de konfigurerte betingelsene som påvirket meldingen.</span><span class="sxs-lookup"><span data-stu-id="dd02e-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="dd02e-110">Hvis du vil ha mer informasjon, [kan du se Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span><span class="sxs-lookup"><span data-stu-id="dd02e-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
