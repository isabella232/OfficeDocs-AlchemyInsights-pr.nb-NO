---
title: Åpne med Explorer fungerer ikke
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538490"
---
# <a name="open-with-explorer-isnt-working"></a>Åpne med Explorer fungerer ikke

Hvis **Åpne med Explorer** eller **visningen i File Explorer** ikke virker Kontroller WebClient-tjenesten er satt til å **kjøre** ved å følge trinnene nedenfor. For eksempel kan det ta lang tid å åpne et SharePoint eller OneDrive bibliotek når tjenesten ikke kjører. 
  
1. I Windows søk-boksen, Skriv inn run, velger du Kjør desktop app, Skriv inn services.msc og deretter **Enter**.
    
2. Rull ned til WebClient-tjenesten, og kontroller **Status** -kolonnen. Hvis statusen for WebClient-tjenesten ikke er **kjører**, Dobbeltklikk tjenesten, klikk **Start**, og klikk deretter **OK**. Aktiver tjenesten, hvis det er nødvendig, ved å velge enten **Manuell** eller **automatisk** i boksen **Oppstartstype** . 
    
> [!NOTE]
> Hvis du vil feilsøke problemer med å åpne i File Explorer, kan du se [åpen i Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Utforsk synkronisering som et bedre alternativ: [Synkroniser SharePoint-filer med den nye OneDrive sync-klienten](https://go.microsoft.com/fwlink/?linkid=871666). 
  

