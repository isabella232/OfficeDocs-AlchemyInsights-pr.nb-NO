---
title: For fellesmappemigreringsgruppe med CompletedWithErrors-status
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043605"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>For fellesmappemigreringsgruppe med CompletedWithErrors-status

Bruk følgende fremgangsmåte for å fullføre den satsvise jobben, og hopp over de store/dårlige varene: 
1. Godkjenne de hoppede varene på migreringsgruppen:

    Set-MigrationBatch \<batchnavn> -ApproveSkippedItems 
2. Bruk følgende kommando til å godkjenne de hoppede elementene på overføringsforespørsler som er "Synkronisert", men ikke fullført:

    $pf=Få-publicfolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i i $pf) {hvis ($i.LargeItemsEncountered -gt 0 -eller $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}
3. Migreringsgruppen og forespørslene skal gjenopptas og fullføres om noen få minutter.

