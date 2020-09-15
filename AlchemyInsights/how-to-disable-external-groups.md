---
title: Slik deaktiverer du eksterne grupper
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704137"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="3bbcd-102">Slik deaktiverer du eksterne grupper</span><span class="sxs-lookup"><span data-stu-id="3bbcd-102">How to disable External Groups</span></span>

<span data-ttu-id="3bbcd-103">Eksterne Yammer-meldinger bruker Exchange-transportprotokoller (etr), et sett med proaktiverte kontroller for å hindre at firma informasjon deles.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="3bbcd-104">Hvis du vil begrense brukere fra å opprette eksterne grupper, må du konfigurere en Exchange transport regel (ETR) og deretter konfigurere Yammer til å bruke Exchange-transport regelen til å blokkere eksterne meldinger.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="3bbcd-105">Når du har opprettet en regel i administrasjons senteret for Exchange Online, følger du denne Fremgangs måten for å angi ETR som skal brukes i Yammer:</span><span class="sxs-lookup"><span data-stu-id="3bbcd-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="3bbcd-106">Logg på Yammer som en bekreftet administrator, og i **administrasjons senteret for Yammer**går du til C **innhold og sikkerhets \> Innstillinger** for sikkerhet.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="3bbcd-107">Velg **Gjennomfør Exchange Online Exchange-transporttilbyderen (etr) i Yammer** under **eksterne meldinger**.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="3bbcd-108">Velg **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-108">Choose **Save**.</span></span>

<span data-ttu-id="3bbcd-109">Hvis du vil ha mer informasjon, kan du se [deaktivere eksterne meldinger i et Yammer-nettverk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="3bbcd-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  