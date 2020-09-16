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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="d5ef5-102">For masse overføring av felles mappe med CompletedWithErrors-status</span><span class="sxs-lookup"><span data-stu-id="d5ef5-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="d5ef5-103">Følg Fremgangs måten nedenfor for å fullføre den satsvise jobben, og hopp over de store/dårlige elementene:</span><span class="sxs-lookup"><span data-stu-id="d5ef5-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="d5ef5-104">Godkjenn de hoppet over elementene på overførings gruppen:</span><span class="sxs-lookup"><span data-stu-id="d5ef5-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="d5ef5-105">Bruk følgende kommando for å godkjenne de hoppet over elementene på overførings forespørsler som er "synkronisert", men ikke fullført:</span><span class="sxs-lookup"><span data-stu-id="d5ef5-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="d5ef5-106">Overførings gruppen og forespørslene skal fortsette og full føres om noen minutter.</span><span class="sxs-lookup"><span data-stu-id="d5ef5-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

