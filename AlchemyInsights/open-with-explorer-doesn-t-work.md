---
title: Åpne med Explorer fungerer ikke
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 164d5fe8c992df825d1f52f19792e1623526c35c58ff2f1e1ab601fdcf5f0f53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011345"
---
# <a name="open-with-explorer-isnt-working"></a>Åpne med Explorer fungerer ikke

Hvis **Åpne med Explorer** eller Vis i **Filutforsker** ikke fungerer, må du kontrollere at WebClient-tjenesten er satt til **Kjører** ved å følge fremgangsmåten nedenfor. Det kan for eksempel ta lang tid å åpne et SharePoint eller OneDrive bibliotek når tjenesten ikke kjører. 
  
1. Skriv inn Windows i søkeboksen, velg Kjør skrivebordsprogrammet, skriv inn services.msc, og velg deretter **Enter**.
    
2. Rull ned til WebClient-tjenesten, og kontroller **Status-kolonnen.** Hvis WebClient-tjenestestatusen ikke **kjører,** dobbeltklikker du tjenesten, **klikker Start** og deretter **OK**. Aktiver tjenesten ved behov ved å velge enten **Manuell** eller **Automatisk** i **Oppstartstype-boksen.** 
    
> [!NOTE]
> Hvis du vil feilsøke problemer med å åpne i Filutforsker, kan [du se Åpne i Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Utforsk synkronisering som et bedre alternativ: [Synkroniser SharePoint filer med den nye OneDrive-synkronisering klienten.](https://go.microsoft.com/fwlink/?linkid=871666) 
  

