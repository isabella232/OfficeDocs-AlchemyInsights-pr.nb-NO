---
title: Skjule fellesmapper
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315434"
---
# <a name="hide-public-folders"></a><span data-ttu-id="08c87-102">Skjule fellesmapper</span><span class="sxs-lookup"><span data-stu-id="08c87-102">Hide public folders</span></span>

<span data-ttu-id="08c87-103">**Slik skjuler du hele fellesmappetreet:**</span><span class="sxs-lookup"><span data-stu-id="08c87-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="08c87-104">Bruk fremgangsmåten i denne [artikkelen til](https://aka.ms/ControlPF) å skjule hele fellesmappetreet for selektive brukere eller alle brukere.</span><span class="sxs-lookup"><span data-stu-id="08c87-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="08c87-105">**Slik skjuler du en bestemt fellesmappe:**</span><span class="sxs-lookup"><span data-stu-id="08c87-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="08c87-106">Legge til tillatelser for brukere som trenger tilgang til fellesmappen</span><span class="sxs-lookup"><span data-stu-id="08c87-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="08c87-107">Fjerne **brukerens standard** fra **tillatelseslisten:**</span><span class="sxs-lookup"><span data-stu-id="08c87-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
