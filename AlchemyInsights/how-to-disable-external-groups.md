---
title: Slik deaktiverer du eksterne grupper
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720777"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="15398-102">Slik deaktiverer du eksterne grupper</span><span class="sxs-lookup"><span data-stu-id="15398-102">How to disable External Groups</span></span>

<span data-ttu-id="15398-103">Yammer eksterne meldinger bruker Exchange Transport Rules (ETRs), et sett med proaktive kontroller for å hindre at firmainformasjon deles.</span><span class="sxs-lookup"><span data-stu-id="15398-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="15398-104">Hvis du vil begrense brukere fra å opprette eksterne grupper, må du konfigurere en Exchange transportregel (ETR), og deretter konfigurere Yammer til å bruke Exchange Transport-regelen til å blokkere eksterne meldinger.</span><span class="sxs-lookup"><span data-stu-id="15398-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="15398-105">Når du har opprettet en regel i administrasjonssenteret for Exchange Online, følger du denne fremgangsmåten for å angi at ETR skal brukes i Yammer:</span><span class="sxs-lookup"><span data-stu-id="15398-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="15398-106">Logg på Yammer som en bekreftet administrator, og gå til **C-innstillinger for \> innholds- og sikkerhetssikkerhet** i **Yammer.**</span><span class="sxs-lookup"><span data-stu-id="15398-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="15398-107">Under **Eksterne meldinger**velger du **Fremhev Exchange Online Exchange Transport Rules (ETRs) i Yammer.**</span><span class="sxs-lookup"><span data-stu-id="15398-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="15398-108">Velg **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="15398-108">Choose **Save**.</span></span>

<span data-ttu-id="15398-109">Hvis du vil ha mer informasjon, kan du se [Deaktivere eksterne meldinger i et Yammer-nettverk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="15398-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  