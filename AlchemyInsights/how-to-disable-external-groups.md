---
title: Slik deaktiverer du eksterne grupper
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 09d8b134a4e99912301aa92c2e989fec9dd30a7b
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656396"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="bda1a-102">Slik deaktiverer du eksterne grupper</span><span class="sxs-lookup"><span data-stu-id="bda1a-102">How to disable External Groups</span></span>

<span data-ttu-id="bda1a-p101">Yammer eksterne meldinger gjelder Exchange Transportregler (ETRs), et sett med proaktiv kontroller for å hindre at selskapet informasjon blir delt. Hvis du vil hindre brukere i å opprette eksterne grupper, må du konfigurere en Exchange transport regel (ETR), og deretter konfigurere Yammer Hvis du vil bruke regelen for Exchange Transport til å blokkere eksternt messaging.</span><span class="sxs-lookup"><span data-stu-id="bda1a-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="bda1a-105">Når du har opprettet en regel i Exchange Online administrasjonssenteret, følger du disse trinnene for å angi ETR å bruke i Yammer:</span><span class="sxs-lookup"><span data-stu-id="bda1a-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="bda1a-106">Logger på Yammer som en kontrollert admin, og **Yammer administrasjonssenteret**, går du til C **Innhaldstype og sikkerhet \> sikkerhetsinnstillinger.**</span><span class="sxs-lookup"><span data-stu-id="bda1a-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="bda1a-107">**Eksterne meldinger**, velg **gjennomføre Exchange Online Exchange Transport reglene (ETRs) i Yammer.**</span><span class="sxs-lookup"><span data-stu-id="bda1a-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="bda1a-108">Velg **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="bda1a-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="bda1a-109">Hvis du vil ha mer informasjon, se [kontrollere eksterne meldinger i Yammer-nettverket med Exchange Transportregler](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="bda1a-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

