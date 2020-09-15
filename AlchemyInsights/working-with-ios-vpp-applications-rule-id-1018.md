---
title: Arbeide med iOS VPP-programmer regel-ID 1018
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
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688955"
---
# <a name="working-with-ios-vpp-applications"></a>Arbeide med iOS VPP-programmer

Les [hvordan du administrerer IOS-apper som er kjøpt via et volum kjøps program med Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) , til å lære om funksjoner, begrensninger og trinn for å bruke Apple Volume kjøps program og støtte for det i Microsoft Intune.
  
 **Vanlige problemer:** «Jeg tilordnet en iOS-app til brukerne mine, men installasjonen mislyktes.»
  
- Dette kan skje hvis ett enkelt VPP-token brukes på tvers av flere administrasjons leverandører av mobil enheter. VPP-tokener fra Apple kan bare brukes med én leverandør. Hvis du har brukt et VPP-token med flere leverandører, må du laste opp tokenet på nytt til Intune.

- Installasjonen kan også mislykkes hvis det totale antallet installasjoner overskrider antall lisenser. Hvis du vil vise en bruks rapport for lisensene dine, kan du gå til siden Intune-lisenser for **Mobilapper** - \> **appene** . Hvis du vil lære hvordan du reviderer lisenser i bruk, kan du se [denne artikkelen.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
