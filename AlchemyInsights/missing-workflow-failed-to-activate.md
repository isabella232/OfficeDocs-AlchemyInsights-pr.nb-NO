---
title: Manglende arbeidsflyt kan ikke aktiveres
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: d703e87f355f05bf4a1d71e5daddce96db988380bb48accc81c95f1ba91fbb2b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065437"
---
# <a name="missing-workflow-failed-to-activate"></a>Manglende arbeidsflyt kan ikke aktiveres

I en Microsoft SharePoint-områdesamling kan du ikke legge til en arbeidsflyt som kan brukes på nytt globalt (for eksempel Godkjenning - SharePoint 2010) i en liste eller et bibliotek.
  
Følg disse trinnene for å løse dette problemet: 
  
1. Åpne rotnettstedet for nettstedssamlingen i SharePoint Designer 2013.
  
2. Velg **Arbeidsflyter** under **Nettstedsobjekter**. 
  
3. Velg **Arbeidsflyt som kan** brukes på nytt i Ny-delen av **Arbeidsflyter-båndet.**  
  
4. Skriv inn navnet ** *Repair2010* **i skjemaet **Opprett** arbeidsflyt som kan brukes på nytt. For **Plattformtype** klikker **du SharePoint 2010-arbeidsflyt**, og deretter klikker du **OK**. 
  
1. Velg Publiser i **Lagre-delen** på **arbeidsflytbåndet.**  
  
2. Velg **Publiser** globalt i Behandle-delen av **arbeidsflytbåndet.**  Velg OK i bekreftelsesdialogboksen som **vises.** 
  
3. Finn rotnettstedet for nettstedssamlingen i en nettleser, og få deretter tilgang til **nettstedsfunksjoner Innstillinger** \> **nettstedssamlinger**. Deretter veksler du **arbeidsflytfunksjonen:** 
  
· Hvis funksjonen er  *aktivert,*  klikker du **Deaktiver,** og deretter klikker du **Aktiver**. 
  
· Hvis funksjonen er  *deaktivert,*  klikker du **Aktiver**. 
  
Hvis du vil ha mer informasjon, kan du se følgende [artikkel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

