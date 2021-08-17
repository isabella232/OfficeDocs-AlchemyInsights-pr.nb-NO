---
title: Arbeide med iOS VPP Applications Rule ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083023"
---
# <a name="working-with-ios-vpp-applications"></a>Arbeide med IOS VPP-programmer

Les Slik administrerer du [iOS-apper](https://docs.microsoft.com/intune/vpp-apps-ios) som er kjøpt via et volumkjøpsprogram med Microsoft Intune for å lære om funksjoner, begrensninger og trinn for å gjøre bruk av Apple Volume Purchase Program og støtte for det i Microsoft Intune.
  
 **Vanlige problemer:** «Jeg tilordnet en IOS VPP-app til brukerne mine, men installasjonen mislyktes.»
  
- Dette kan skje hvis ett enkelt VPP-token brukes på tvers av flere leverandører av administrasjon av mobilenheter. VPP-tokener fra Apple kan bare brukes med én leverandør. Hvis du brukte et VPP-token med flere leverandører, må du laste opp tokenet på nytt til Intune.

- Installasjonen kan også mislykkes hvis det totale antallet installasjoner overskrider antall lisenser. Hvis du vil vise en bruksrapport for lisensene dine, kan du gå til siden Lisenser for **Intune-mobilapper.** \>  Hvis du vil lære hvordan du gjenvinner lisenser i bruk, kan du se [denne artikkelen.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
