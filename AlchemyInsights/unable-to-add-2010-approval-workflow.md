---
title: Kan ikke legge til 2010 godkjenningsarbeidsflyt
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 11ba9bf04f826b0d7465a9a81a36c327e79f4d13
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049562"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Kan ikke legge til 2010 godkjenningsarbeidsflyt

I en områdesamling for Microsoft SharePoint kan du ikke legge til en globalt gjenbrukbar arbeidsflyt (for eksempel "godkjenning – SharePoint 2010") i en liste eller et bibliotek.
  
Hvis du vil løse dette problemet, følger du denne fremgangsmåten: 
  
1. Åpne det primære webområdet for områdesamlingen i SharePoint Designer 2013.
  
2. Velg **arbeidsflyter**under **områdeobjekter**. 
  
3. Velg **gjenbrukbar arbeidsflyt**i den **nye** delen av båndet **arbeidsflyter** . 
  
4. I skjemaet **Opprett gjenbrukbar arbeidsflyt** skriver du inn navnet * * *Repair2010* * *. For **plattform type**, klikker du **SharePoint 2010 arbeidsflyt**, og klikk deretter **OK**. 
  
1. Velg **Publiser**i **Lagre** -delen av **arbeidsflyt** båndet. 
  
2. Velg **Publiser globalt**i **Behandle** -delen av **arbeidsflyt** båndet. Velg **OK**i bekreftelsesdialogboksen som vises. 
  
3. I en webleser finner du rotwebområdet for områdesamlingen, og deretter får du tilgang til **områdesamlingsfunksjoner** **for områdeinnstillinger** \> . Aktiver/Deaktiver funksjonen **arbeidsflyter** : 
  
· Hvis funksjonen er *aktivert* , klikker du **Deaktiver,** og klikk deretter **Aktiver**. 
  
· Hvis funksjonen er *deaktivert* , klikker du **Aktiver**. 
  
For mer informasjon henvises til følgende [artikkel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

