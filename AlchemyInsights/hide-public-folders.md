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
# <a name="hide-public-folders"></a>Skjule fellesmapper

**Slik skjuler du hele fellesmappetreet:**

Bruk fremgangsmåten i denne [artikkelen til](https://aka.ms/ControlPF) å skjule hele fellesmappetreet for selektive brukere eller alle brukere.

**Slik skjuler du en bestemt fellesmappe:**

1. Legge til tillatelser for brukere som trenger tilgang til fellesmappen

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Fjerne **brukerens standard** fra **tillatelseslisten:**

    `Remove-PublicFolderClientPermission \test1 -User Default`
