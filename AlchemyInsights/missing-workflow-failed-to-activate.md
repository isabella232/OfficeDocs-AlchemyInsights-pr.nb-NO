---
title: Manglende arbeids flyt kan ikke aktivere
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667095"
---
# <a name="missing-workflow-failed-to-activate"></a>Manglende arbeids flyt kan ikke aktivere

I en Microsoft SharePoint-områdesamling kan du ikke legge til en global gjenbrukbar arbeids flyt (for eksempel "godkjenning-SharePoint 2010") i en liste eller et bibliotek.
  
Følg denne Fremgangs måten for å løse dette problemet: 
  
1. Åpne rot nettstedet for nettsteds samlingen i SharePoint Designer 2013.
  
2. Velg **arbeids flyter**under **område objekter**. 
  
3. Velg **gjenbrukbar arbeids flyt**i den **nye** delen av **arbeids flyt** båndet. 
  
4. Skriv inn navnet * * *Repair2010* * * i skjemaet **Opprett gjenbrukbar arbeids flyt** . For **plattform type**klikker du **SharePoint 2010-arbeidsflyt**, og deretter klikker du **OK**. 
  
1. Velg **Publiser**i **Lagre** -delen på **arbeids flyt** båndet. 
  
2. Velg **Publiser globalt**i delen **Behandle** i **arbeids flyt** båndet. Velg **OK**i bekreftelses dialog boksen som vises. 
  
3. Finn rot nettstedet for nettsteds samlingen i en nett leser, og få deretter tilgang **Site Settings** til område \> **samlings funksjoner**for nettsteds innstillinger. Deretter aktiverer/deaktiverer du **arbeidsflyter** -funksjonen: 
  
· Hvis funksjonen er  *aktivert*  , klikker du **Deaktiver,** og deretter klikker du **Aktiver**. 
  
· Hvis funksjonen er  *deaktivert*  , klikker du **Aktiver**. 
  
Hvis du vil ha mer informasjon, kan du se følgende [artikkel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

