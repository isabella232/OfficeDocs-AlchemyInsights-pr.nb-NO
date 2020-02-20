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
# <a name="restore-a-deleted-public-folder"></a>Gjenopprette en slettet fellesmappe

**Slik gjenoppretter du slettede elementer fra en fellesmappe:**

- Se [Du kan ikke gjenopprette slettede elementer fra en fellesmappe som ikke er sendt fra e-post i Outlook-2016](https://aka.ms/pfrec).
 
**Slik gjenoppretter du en slettet fellesmappe (av en hvilken som helst type):** 

- Bruk følgende EXO PowerShell-kommando:

    Syntaks:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Eksempel: Følgende kommando gjenoppretter undermappe1 og plasserer den under \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Se [Gjenopprette en slettet fellesmappe](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) hvis du vil ha mer informasjon.
