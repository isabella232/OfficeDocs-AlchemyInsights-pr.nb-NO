---
title: Feilsøke karantene tilstand
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7853"
- "9004348"
ms.openlocfilehash: 3ee932b7788f4aff3c8bc762c5c917124edfe065
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949916"
---
# <a name="troubleshoot-quarantine-state"></a><span data-ttu-id="3fd28-102">Feilsøke karantene tilstand</span><span class="sxs-lookup"><span data-stu-id="3fd28-102">Troubleshoot quarantine state</span></span>

<span data-ttu-id="3fd28-103">Klar gjørings tjenesten for Azure Active Directory (AD) overvåker tilstanden til konfigurasjonen.</span><span class="sxs-lookup"><span data-stu-id="3fd28-103">The Azure Active Directory (AD) provisioning service monitors the health of your configuration.</span></span> <span data-ttu-id="3fd28-104">Den plasserer også ikke-tilstands apper i en **karantene** tilstand.</span><span class="sxs-lookup"><span data-stu-id="3fd28-104">It also places unhealthy apps in a **quarantine** state.</span></span> <span data-ttu-id="3fd28-105">Hvis de fleste av samtalene som utføres mot mål systemet konsekvent mislykkes, blir klar gjørings jobben merket som **i karantene**.</span><span class="sxs-lookup"><span data-stu-id="3fd28-105">If most, or all, of the calls made against the target system consistently fail, then the provisioning job is marked as **in quarantine**.</span></span> <span data-ttu-id="3fd28-106">Et eksempel på en feil **melding er en feil som er mottatt, på grunn av ugyldige administrator legitimasjoner**.</span><span class="sxs-lookup"><span data-stu-id="3fd28-106">An example of a failure is **an error received because of invalid admin credentials**.</span></span> <span data-ttu-id="3fd28-107">Hvis du vil ha mer informasjon, kan du se [program klar gjøring i karantene status](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-quarantine-status).</span><span class="sxs-lookup"><span data-stu-id="3fd28-107">For more information, see [Application provisioning in quarantine status](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-quarantine-status).</span></span>

<span data-ttu-id="3fd28-108">Hvis du vil feilsøke Sky BAS ert synkronisering, kan du se [klargjøre problemer i karantene](https://docs.microsoft.com/azure/active-directory/cloud-sync/how-to-troubleshoot#provisioning-quarantined-problems).</span><span class="sxs-lookup"><span data-stu-id="3fd28-108">To troubleshoot cloud sync, see [Provisioning quarantined problems](https://docs.microsoft.com/azure/active-directory/cloud-sync/how-to-troubleshoot#provisioning-quarantined-problems).</span></span> 
