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
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063706"
---
# <a name="restore-a-deleted-public-folder"></a>Gjenopprette en slettet fellesmappe

**Slik gjenoppretter du slettede elementer fra en fellesmappe:**

- Se [Du kan ikke gjenopprette slettede elementer fra en fellesmappe som ikke er sendt fra e-post i Outlook-2016](https://aka.ms/pfrec).
 
**Slik gjenoppretter du en slettet fellesmappe (av en hvilken som helst type):** 

- Bruk følgende EXO PowerShell-kommando:

    Syntaks:

    >$pf=Bli-publicmappe \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Navn -eq\<" name_of_deleted_public_Folder"}; Set-PublicFolder $pf.identity \<-Bane der mappen skal gjenopprettes>

    Eksempel: Følgende kommando gjenoppretter undermappe1 og plasserer den under \Parent1:

    >$pf=Bli-publicmappe \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Navn -eq "Undermappe1"}; Set-PublicFolder $pf.identity -Bane \Parent1

Se [Gjenopprette en slettet fellesmappe](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) hvis du vil ha mer informasjon.
