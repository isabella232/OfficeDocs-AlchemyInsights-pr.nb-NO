---
title: Replikasett
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714252"
---
# <a name="replica-set"></a><span data-ttu-id="c6454-102">Replikasett</span><span class="sxs-lookup"><span data-stu-id="c6454-102">Replica set</span></span>

<span data-ttu-id="c6454-103">AADDS kalles også det administrerte domenet.</span><span class="sxs-lookup"><span data-stu-id="c6454-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="c6454-104">Det er faktisk to domenekontrollere som kjøres og vedlikeholdes av serverserveren.</span><span class="sxs-lookup"><span data-stu-id="c6454-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="c6454-105">De to DC-ene inkluderer én hoved-DC og én replikerings-DC.</span><span class="sxs-lookup"><span data-stu-id="c6454-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="c6454-106">Sikkerhetskopier i AADDS (administrert domene) er en automatisert prosess som administreres av Azure-plattformen.</span><span class="sxs-lookup"><span data-stu-id="c6454-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="c6454-107">Hvis det oppstår et problem med det administrerte domenet, kan Azure-støtte hjelpe deg med å gjenopprette fra sikkerhetskopiering.</span><span class="sxs-lookup"><span data-stu-id="c6454-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="c6454-108">Du oppretter hvert replikasett i et virtuelt nettverk.</span><span class="sxs-lookup"><span data-stu-id="c6454-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="c6454-109">Hvert virtuelle nettverk må nodenett til alle andre virtuelle nettverk som er vert for et administrert domenes replikeringssett.</span><span class="sxs-lookup"><span data-stu-id="c6454-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="c6454-110">Denne konfigurasjonen oppretter en nettverkstopologi for nett som støtter katalogreplikering.</span><span class="sxs-lookup"><span data-stu-id="c6454-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="c6454-111">Et virtuelt nettverk kan støtte flere replikasett forutsatt at hvert replikasett er i et annet virtuelt delnett.</span><span class="sxs-lookup"><span data-stu-id="c6454-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="c6454-112">Hvis du vil ha mer informasjon om replikasett, kan du [se Concepts Replica sets.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)</span><span class="sxs-lookup"><span data-stu-id="c6454-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
