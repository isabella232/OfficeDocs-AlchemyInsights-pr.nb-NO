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
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943384"
---
# <a name="restore-a-deleted-public-folder"></a>Gjenopprette en slettet fellesmappe

**Slik gjenoppretter du slettede elementer fra en fellesmappe:**

- Se Du kan ikke gjenopprette slettede elementer fra en fellesmappe som ikke er [e-post, i Outlook 2016](https://aka.ms/pfrec).
 
**Slik gjenoppretter du en slettet fellesmappe (av en hvilken som helst type):** 

- Bruk følgende EXO PowerShell-kommando:

    Syntaks:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Eksempel: Følgende kommando gjenoppretter Undermappe1 og plasserer den under \Overordnet1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Se [Gjenopprette en slettet fellesmappe hvis du](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) vil ha mer informasjon.
