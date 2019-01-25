---
title: Manglende arbeidsflyten kan ikke aktivere
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 33b92c2cae1f641b0cd88c82fd4ae5e8632d76c2
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29481263"
---
# <a name="missing-workflow-failed-to-activate"></a>Manglende arbeidsflyten kan ikke aktivere

Du kan legge et globalt gjenbrukbar arbeidsflyt (for eksempel "godkjenning - SharePoint 2010") til lister eller biblioteker i en områdesamling for Microsoft SharePoint.
  
Hvis du vil løse dette problemet, gjør du følgende: 
  
1. Åpne webområdet til roten av områdesamlingen i SharePoint Designer 2013.
  
2. Under **Områdeobjekter**, velger du **arbeidsflyter**. 
  
3. Velg **Gjenbrukbare arbeidsflyt**i **Ny** -delen av båndet **arbeidsflyter** . 
  
4. Angi navnet på skjemaet **Opprett gjenbrukbare arbeidsflyten** ** *Repair2010* **. Klikk **SharePoint 2010 arbeidsflyt**for **Plattformen**, og klikk deretter **OK**. 
  
1. Velg **Publiser**i delen **Lagre** **arbeidsflyt** -båndet. 
  
2. Velg **Publiser globalt**i delen **Behandle** **arbeidsflyt** -båndet. I bekreftelsesdialogboksen som vises, velger du **OK**. 
  
3. Finne webområdet til roten av områdesamlingen i en webleser, og deretter bruker du **Områdeinnstillinger** \> **Funksjoner i områdesamling**. Deretter Aktiver/deaktiver funksjonen **arbeidsflyter** : 
  
· Hvis funksjonen er *aktivert* , klikker du **Deaktiver,** og klikk deretter **Aktiver**. 
  
· Hvis funksjonen er *deaktivert* , klikker du **Aktiver**. 
  
For mer informasjon kan du se følgende [artikkel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

