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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695856"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="c33bd-102">Løse transportregler</span><span class="sxs-lookup"><span data-stu-id="c33bd-102">Fix transport rules</span></span>

<span data-ttu-id="c33bd-103">En egendefinert e-postflytregel har påvirket denne meldingen.</span><span class="sxs-lookup"><span data-stu-id="c33bd-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="c33bd-104">Hvis du vil se den nøyaktige regelen, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="c33bd-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="c33bd-105">Legg merke til GUID-en eller  policynavnet under **Tilleggsinformasjon** i innsendingsresultatene. </span><span class="sxs-lookup"><span data-stu-id="c33bd-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="c33bd-106">Start Skall for administrasjon av Exchange.</span><span class="sxs-lookup"><span data-stu-id="c33bd-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="c33bd-107">Hvis du vil ha mer informasjon, [kan du se Åpne Exchange Management Shell.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="c33bd-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="c33bd-108">Kjør denne kommandoen (ved hjelp av GUID fra **innsendingen): Get-TransportRule -identity "GUID"** | fl \* Description\*</span><span class="sxs-lookup"><span data-stu-id="c33bd-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="c33bd-109">Se gjennom beskrivelsen for å se de konfigurerte betingelsene som påvirket meldingen.</span><span class="sxs-lookup"><span data-stu-id="c33bd-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="c33bd-110">Hvis du vil ha mer informasjon, kan du [se Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)</span><span class="sxs-lookup"><span data-stu-id="c33bd-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
