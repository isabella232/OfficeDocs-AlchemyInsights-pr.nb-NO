---
title: For overføringsgruppen for fellesmappe med CompletedWithErrors-status
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812473"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>For overføringsgruppen for fellesmappe med CompletedWithErrors-status

Bruk følgende fremgangsmåte for å fullføre jobben og hoppe over de store/ugyldige elementene: 
1. Godkjenn elementene som er hoppet over i overføringsgruppen:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Bruk følgende kommando til å godkjenne de hoppede elementene på overføringsforespørsler som er synkronisert, men ikke fullført:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Overføringsgruppen og forespørslene skal gjenopptas og fullføres om noen minutter.

