---
title: 'Feilsøke talepost '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679110"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="70836-102">Feilsøke talepost</span><span class="sxs-lookup"><span data-stu-id="70836-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="70836-103">Kontroller at funksjonen opptatt på opptatt er bevisst.</span><span class="sxs-lookup"><span data-stu-id="70836-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="70836-104">Hvis denne funksjonen ikke er nødvendig på denne brukeren:</span><span class="sxs-lookup"><span data-stu-id="70836-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="70836-105">Gå til [administrasjons senteret for Teams](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="70836-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="70836-106">Gå til venstre tog, og  >  **Ring retnings linjer** for samtaler  >  **Behandle policyer** i **anrops policyen**.</span><span class="sxs-lookup"><span data-stu-id="70836-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="70836-107">Velg **Behandle brukere**.</span><span class="sxs-lookup"><span data-stu-id="70836-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="70836-108">Søk etter bruker og endre anrops policyen til en som har vært **opptatt er tilgjengelig når du er i en samtale** . </span><span class="sxs-lookup"><span data-stu-id="70836-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="70836-109">Klikk på **Bruk**.</span><span class="sxs-lookup"><span data-stu-id="70836-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="70836-110">Endringer i policyer kan ha opptil 24 timer å replisere.</span><span class="sxs-lookup"><span data-stu-id="70836-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="70836-111">Hvis du vil ha mer informasjon om denne funksjonen, kan du se: [opptatt på opptatt er tilgjengelig når du er i en samtale](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="70836-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
