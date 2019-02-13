---
title: Slik deaktiverer du eksterne grupper
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4d911c319c3e8e327f9b3af3ba67816e646bc468
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29899145"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="d7c19-102">Slik deaktiverer du eksterne grupper</span><span class="sxs-lookup"><span data-stu-id="d7c19-102">How to disable External Groups</span></span>

<span data-ttu-id="d7c19-p101">Yammer eksterne meldinger gjelder Exchange Transportregler (ETRs), et sett med proaktiv kontroller for å hindre at selskapet informasjon blir delt. Hvis du vil hindre brukere i å opprette eksterne grupper, må du konfigurere en Exchange transport regel (ETR), og deretter konfigurere Yammer Hvis du vil bruke regelen for Exchange Transport til å blokkere eksternt messaging.</span><span class="sxs-lookup"><span data-stu-id="d7c19-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="d7c19-105">Når du har opprettet en regel i Exchange Online administrasjonssenteret, følger du disse trinnene for å angi ETR å bruke i Yammer:</span><span class="sxs-lookup"><span data-stu-id="d7c19-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="d7c19-106">Logger på Yammer som en kontrollert admin, og **Yammer administrasjonssenteret**, går du til C **Innhaldstype og sikkerhet \> sikkerhetsinnstillinger.**</span><span class="sxs-lookup"><span data-stu-id="d7c19-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="d7c19-107">**Eksterne meldinger**, velg **gjennomføre Exchange Online Exchange Transport reglene (ETRs) i Yammer.**</span><span class="sxs-lookup"><span data-stu-id="d7c19-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="d7c19-108">Velg **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="d7c19-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="d7c19-109">Hvis du vil ha mer informasjon, se [kontrollere eksterne meldinger i Yammer-nettverket med Exchange Transportregler](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="d7c19-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

