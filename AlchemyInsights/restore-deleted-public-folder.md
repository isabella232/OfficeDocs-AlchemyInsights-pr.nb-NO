---
title: Gjenopprette en slettet fellesmappe
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
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809448"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="29100-102">Gjenopprette en slettet fellesmappe</span><span class="sxs-lookup"><span data-stu-id="29100-102">Restore a deleted public folder</span></span>

<span data-ttu-id="29100-103">**Slik gjenoppretter du slettede elementer fra en fellesmappe:**</span><span class="sxs-lookup"><span data-stu-id="29100-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="29100-104">Se Du kan ikke gjenopprette slettede elementer fra en fellesmappe som ikke er [e-post, i Outlook 2016.](https://aka.ms/pfrec)</span><span class="sxs-lookup"><span data-stu-id="29100-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="29100-105">**Slik gjenoppretter du en slettet fellesmappe (av en hvilken som helst type):**</span><span class="sxs-lookup"><span data-stu-id="29100-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="29100-106">Bruk følgende EXO PowerShell-kommando:</span><span class="sxs-lookup"><span data-stu-id="29100-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="29100-107">Syntaks:</span><span class="sxs-lookup"><span data-stu-id="29100-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="29100-108">Eksempel: Følgende kommando gjenoppretter Undermappe1 og plasserer den under \Overordnet1:</span><span class="sxs-lookup"><span data-stu-id="29100-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="29100-109">Se [Gjenopprette en slettet fellesmappe hvis du](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) vil ha mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="29100-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
