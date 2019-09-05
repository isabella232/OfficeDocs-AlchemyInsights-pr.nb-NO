---
title: Manglende arbeidsflyt ble ikke aktivert
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753805"
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
  

