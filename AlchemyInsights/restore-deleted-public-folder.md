---
title: Gjenopprette en slettet fellesmappe
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
- "3488"
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158527"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="d8ae6-102">Gjenopprette en slettet fellesmappe</span><span class="sxs-lookup"><span data-stu-id="d8ae6-102">Restore a deleted public folder</span></span>

<span data-ttu-id="d8ae6-103">**Slik gjenoppretter du slettede elementer fra en fellesmappe:**</span><span class="sxs-lookup"><span data-stu-id="d8ae6-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="d8ae6-104">Se [Du kan ikke gjenopprette slettede elementer fra en fellesmappe som ikke er sendt fra e-post i Outlook-2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="d8ae6-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="d8ae6-105">**Slik gjenoppretter du en slettet fellesmappe (av en hvilken som helst type):**</span><span class="sxs-lookup"><span data-stu-id="d8ae6-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="d8ae6-106">Bruk følgende EXO PowerShell-kommando:</span><span class="sxs-lookup"><span data-stu-id="d8ae6-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="d8ae6-107">Syntaks:</span><span class="sxs-lookup"><span data-stu-id="d8ae6-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="d8ae6-108">Eksempel: Følgende kommando gjenoppretter undermappe1 og plasserer den under \Parent1:</span><span class="sxs-lookup"><span data-stu-id="d8ae6-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="d8ae6-109">Se [Gjenopprette en slettet fellesmappe](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) hvis du vil ha mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="d8ae6-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
