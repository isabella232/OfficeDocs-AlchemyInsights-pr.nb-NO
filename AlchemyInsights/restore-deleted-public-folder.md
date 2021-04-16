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
# <a name="restore-a-deleted-public-folder"></a>Gjenopprette en slettet fellesmappe

**Slik gjenoppretter du slettede elementer fra en fellesmappe:**

- Se Du kan ikke gjenopprette slettede elementer fra en fellesmappe som ikke er [e-post, i Outlook 2016.](https://aka.ms/pfrec)
 
**Slik gjenoppretter du en slettet fellesmappe (av en hvilken som helst type):** 

- Bruk følgende EXO PowerShell-kommando:

    Syntaks:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Eksempel: Følgende kommando gjenoppretter Undermappe1 og plasserer den under \Overordnet1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Se [Gjenopprette en slettet fellesmappe hvis du](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) vil ha mer informasjon.
