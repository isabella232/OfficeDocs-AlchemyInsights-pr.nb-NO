---
title: Slik deaktiverer du eksterne grupper
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36739502"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="a1aa5-102">Slik deaktiverer du eksterne grupper</span><span class="sxs-lookup"><span data-stu-id="a1aa5-102">How to disable External Groups</span></span>

<span data-ttu-id="a1aa5-103">Yammer eksterne meldinger bruker Exchange transport Rules (ETRs), et sett med proaktive kontroller for å hindre at firmainformasjon blir delt.</span><span class="sxs-lookup"><span data-stu-id="a1aa5-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="a1aa5-104">For å begrense brukere fra å opprette eksterne grupper, må du konfigurere en Exchange transport-regel (ETR), og deretter konfigurere Yammer til å bruke Exchange transport-regelen til å blokkere eksterne meldinger.</span><span class="sxs-lookup"><span data-stu-id="a1aa5-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="a1aa5-105">Når du har opprettet en regel i Exchange Online administrasjonssenteret, følger du denne fremgangsmåten for å angi ETR skal brukes i Yammer:</span><span class="sxs-lookup"><span data-stu-id="a1aa5-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="a1aa5-106">Logg på Yammer som en verifisert admin, og i **administrasjonssenteret for Yammer**, gå til C- **innhold og sikkerhets \> innstillinger for sikkerhet.**</span><span class="sxs-lookup"><span data-stu-id="a1aa5-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="a1aa5-107">Under **eksterne meldinger**velger **du Gjennomfør Exchange Online Exchange transport Rules (ETRs) i Yammer.**</span><span class="sxs-lookup"><span data-stu-id="a1aa5-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="a1aa5-108">Velg **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="a1aa5-108">Choose **Save**.</span></span>

<span data-ttu-id="a1aa5-109">Hvis du vil ha mer informasjon, kan du se [deaktivere eksterne meldinger i et Yammer-nettverk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="a1aa5-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  