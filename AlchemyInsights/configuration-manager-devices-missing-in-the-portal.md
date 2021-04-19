---
title: Enheter for Configuration Manager mangler i portalen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817253"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="aee9a-102">Enheter for Configuration Manager mangler i portalen</span><span class="sxs-lookup"><span data-stu-id="aee9a-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="aee9a-103">For at enhetssynkronisering skal fungere, må [nødvendige Internett-endepunkter](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) kunne nås fra den lokale serveren, som er vert for kontrollen til tjenestetilkobling.</span><span class="sxs-lookup"><span data-stu-id="aee9a-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="aee9a-104">Hvis du vil feilsøke enhetssynkronisering, kan du se **CMGatewaySyncUploadWorker. log** som befinner seg på punktet for tjenestetilkobling.</span><span class="sxs-lookup"><span data-stu-id="aee9a-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="aee9a-105">Finn ut mer om [Tenant-tilknyttning i Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="aee9a-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
