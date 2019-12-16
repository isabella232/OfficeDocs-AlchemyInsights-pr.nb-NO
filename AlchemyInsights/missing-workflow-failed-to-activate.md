---
title: Manglende arbeidsflyt ble ikke aktivert
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 3df1ddc1059c4cd6cc3f9f42dc157d20be79a63a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052622"
---
# <a name="missing-workflow-failed-to-activate"></a>Manglende arbeidsflyt ble ikke aktivert

I en områdesamling for Microsoft SharePoint kan du ikke legge til en globalt gjenbrukbar arbeidsflyt (for eksempel "godkjenning – SharePoint 2010") i en liste eller et bibliotek.
  
Hvis du vil løse dette problemet, følger du denne fremgangsmåten: 
  
1. Åpne det primære webområdet for områdesamlingen i SharePoint Designer 2013.
  
2. Velg **arbeidsflyter**under **områdeobjekter**. 
  
3. Velg **gjenbrukbar arbeidsflyt**i den **nye** delen av båndet **arbeidsflyter** . 
  
4. I skjemaet **Opprett gjenbrukbar arbeidsflyt** skriver du inn navnet * * *Repair2010* * *. For **plattform type**, klikker du **SharePoint 2010 arbeidsflyt**, og klikk deretter **OK**. 
  
1. Velg **Publiser**i **Lagre** -delen av **arbeidsflyt** båndet. 
  
2. Velg **Publiser globalt**i **Behandle** -delen av **arbeidsflyt** båndet. Velg **OK**i bekreftelsesdialogboksen som vises. 
  
3. I en webleser finner du rotwebområdet for områdesamlingen, og deretter får du tilgang til **områdesamlingsfunksjoner** **for områdeinnstillinger** \> . Deretter aktiverer du funksjonen **arbeidsflyter** : 
  
· Hvis funksjonen er *aktivert* , klikker du **Deaktiver,** og klikk deretter **Aktiver**. 
  
· Hvis funksjonen er *deaktivert* , klikker du **Aktiver**. 
  
For mer informasjon henvises til følgende [artikkel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

