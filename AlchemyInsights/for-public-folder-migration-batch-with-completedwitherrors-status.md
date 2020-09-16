---
title: For masse overføring av felles mappe med CompletedWithErrors-status
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744122"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>For masse overføring av felles mappe med CompletedWithErrors-status

Følg Fremgangs måten nedenfor for å fullføre den satsvise jobben, og hopp over de store/dårlige elementene: 
1. Godkjenn de hoppet over elementene på overførings gruppen:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Bruk følgende kommando for å godkjenne de hoppet over elementene på overførings forespørsler som er "synkronisert", men ikke fullført:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Overførings gruppen og forespørslene skal fortsette og full føres om noen minutter.

