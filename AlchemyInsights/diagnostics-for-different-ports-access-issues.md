---
title: Diagnostikk for ulike tilgangsproblemer for porter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035778"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="58a7c-102">Diagnostikk for ulike tilgangsproblemer for porter</span><span class="sxs-lookup"><span data-stu-id="58a7c-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="58a7c-103">Gjør følgende for å løse de ulike porttilgangsproblemene:</span><span class="sxs-lookup"><span data-stu-id="58a7c-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="58a7c-104">Stopp/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span><span class="sxs-lookup"><span data-stu-id="58a7c-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="58a7c-105">Kontroller nettverksinnstillingene for VM for å finne ut om du har nettverkssikkerhetsgrupper (NSGs) som blokkerer trafikk.</span><span class="sxs-lookup"><span data-stu-id="58a7c-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="58a7c-106">Du kan også bruke Kontrollverktøy for IP-flyt i [Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) til å se etter NSGs som blokkerer trafikk, User-Defined Routes (UDRs) omdirigere trafikken tilbake til lokalt (Standardrute' 0.0.0.0/0) eller til et nettverksutstyr.</span><span class="sxs-lookup"><span data-stu-id="58a7c-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="58a7c-107">Hvis du fremdeles opplever problemer etter at du har prøvd fremgangsmåten ovenfor, kan du angi VM-navnet og TCP-porten du prøver å sende e-post på for ytterligere diagnose.</span><span class="sxs-lookup"><span data-stu-id="58a7c-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="58a7c-108">**Anbefalte dokumenter**</span><span class="sxs-lookup"><span data-stu-id="58a7c-108">**Recommended Documents**</span></span>

[<span data-ttu-id="58a7c-109">Begrensninger og anbefalinger for sending av utgående e-post over port 25</span><span class="sxs-lookup"><span data-stu-id="58a7c-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)