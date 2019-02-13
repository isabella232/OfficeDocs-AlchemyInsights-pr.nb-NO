---
title: Arbeide med iOS VPP programmer regel-Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917505"
---
# <a name="working-with-ios-vpp-applications"></a>Arbeide med iOS VPP-programmer

Les [hvordan du administrerer iOS apps kjøpt via et volum Kjøpsprogram med Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) å lære om funksjoner, betingelser og trinn for å gjøre bruk av Apple volum kjøpe programmet og støtte for den i Microsoft Intune. 
  
 **Vanlige problemer:** "Jeg har tilordnet en iOS VPP app til brukerne, men installasjonen mislyktes". 
  
- Dette kan skje hvis et enkelt VPP-token brukes på tvers av flere leverandører av mobil enhet management. VPP-tokener fra Apple kan bare brukes med én leverandør. Hvis du brukte et VPP-token med flere leverandører, må du laste opp token til Intune på nytt.
    
- Installasjonen kan også mislykkes hvis det totale antallet installasjoner overstiger antall lisenser. Hvis du vil vise en Bruksrapport for lisensene, går du til **Intune Mobile apps** \> **App lisenser** -siden. Hvis du vil lære å gjenvinne lisenser i bruk, kan du se [denne artikkelen.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
    

