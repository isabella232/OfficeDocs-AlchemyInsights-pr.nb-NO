---
title: Manglende arbeidsflyt kan ikke aktiveres
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762110"
---
# <a name="missing-workflow-failed-to-activate"></a>Manglende arbeidsflyt kan ikke aktiveres

I en Microsoft SharePoint-områdesamling kan du ikke legge til en globalt gjenbrukbar arbeidsflyt (for eksempel "Godkjenning - SharePoint 2010") i en liste eller et bibliotek.
  
Hvis du vil løse dette problemet, gjør du følgende: 
  
1. Åpne rotwebområdet for områdesamlingen i SharePoint Designer 2013.
  
2. Velg **Arbeidsflyter**under **Områdeobjekter**. 
  
3. Velg **Arbeidsflyt** som **Workflows** **kan brukes på nytt**. 
  
4. I skjemaet **Opprett ny brukbar arbeidsflyt** skriver du inn navnet ** *Repair2010* **. Klikk **SharePoint 2010-arbeidsflyt**for **Plattformtype**, og klikk deretter **OK**. 
  
1. Velg **Publiser**i **Lagre-delen** på **Arbeidsflyt-båndet.** 
  
2. Velg **Publiser globalt**i **Behandle-delen** på **Arbeidsflyt-båndet.** Velg **OK**i bekreftelsesdialogboksen som vises. 
  
3. Finn rotwebområdet for områdesamlingen i en nettleser, og få deretter tilgang til funksjoner **for områdeinnstillinger** \> **områdesamling**. Deretter veksler du **arbeidsflytfunksjonen:** 
  
· Hvis funksjonen er *Aktivert* , klikker du **Deaktiver,** og deretter klikker du **Aktiver**. 
  
· Hvis funksjonen er *Deaktivert* , klikker du **Aktiver**. 
  
Hvis du vil ha mer informasjon, kan du se følgende [artikkel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

