---
title: Åpen med Explorer fungerer ikke
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713043"
---
# <a name="open-with-explorer-isnt-working"></a>Åpne med Explorer fungerer ikke

Hvis **Åpne med Explorer** eller Vis i **Filutforsker** ikke fungerer, må du kontrollere at WebClient-tjenesten er satt til **Å kjøre** ved å følge trinnene nedenfor. Det kan for eksempel ta lang tid å åpne et SharePoint- eller OneDrive-bibliotek når tjenesten ikke kjører. 
  
1. Skriv inn kjør i Søkeboksen i Windows, velg Kjør skrivebord-appen, skriv inn services.msc, og velg deretter **Enter**.
    
2. Bla ned til WebClient-tjenesten, og kontroller **Status-kolonnen.** Hvis WebClient-tjenestestatusen ikke **kjører**, dobbeltklikker du tjenesten, klikker **Start**, og deretter klikker du **OK**. Aktiver om nødvendig tjenesten ved å velge **manuell** eller **automatisk** i **Oppstartstype-boksen.** 
    
> [!NOTE]
> Hvis du vil feilsøke problemer med å åpne filutforsker, kan du se [Åpne i Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Utforsk synkronisering som et bedre alternativ: [Synkroniser SharePoint-filer med den nye OneDrive-synkroniseringsklienten](https://go.microsoft.com/fwlink/?linkid=871666). 
  

