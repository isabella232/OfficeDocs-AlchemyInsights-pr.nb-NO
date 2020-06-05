---
title: Kan ikke legge til arbeidsflyt for godkjenning av 2010
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: f40716dd399fe7bea1b606cd725676268dc0a66d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582856"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Kan ikke legge til arbeidsflyt for godkjenning av 2010

I en Microsoft SharePoint-områdesamling kan du ikke legge til en arbeidsflyt som kan brukes på nytt (for eksempel "Godkjenning - SharePoint 2010") i en liste eller et bibliotek.
  
Hvis du vil løse dette problemet, gjør du følgende: 
  
1. Åpne rotwebområdet for områdesamlingen i SharePoint Designer 2013.
  
2. Velg **Arbeidsflyter**under **Områdeobjekter**. 
  
3. Velg Arbeidsflyt som kan brukes på nytt, i **Ny-delen** på **Arbeidsflyter-båndet.** **Workflows** 
  
4. I skjemaet **Opprett arbeidsflyt som kan brukes på nytt,** skriver du inn navnet ** *Repair2010* **. Klikk Arbeidsflyt for **SharePoint 2010**for **Plattformtype**, og klikk deretter **OK**. 
  
1. Velg **Publiser**under **Lagre** på **Arbeidsflyt-båndet.** 
  
2. Velg **Publiser globalt i** **Behandle-delen** på **Arbeidsflyt-båndet.** Velg **OK**i bekreftelsesdialogboksen som vises. 
  
3. Finn rotnettstedet for områdesamlingen i en nettleser, **Site Settings** og få deretter tilgang til \> **funksjoner for områdeinnstillinger områdesamling**. Aktiver/deaktiver **arbeidsflytfunksjonen:** 
  
· Hvis funksjonen er *Aktivert* , klikker du **Deaktiver,** og klikk deretter **Aktiver**. 
  
· Hvis funksjonen er *Deaktivert* , klikker du **Aktiver**. 
  
Hvis du vil ha mer informasjon, kan du se følgende [artikkel.](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)
  

