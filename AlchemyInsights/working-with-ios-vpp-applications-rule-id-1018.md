---
title: Arbeide med iOS VPP-programmer Regel-ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719966"
---
# <a name="working-with-ios-vpp-applications"></a>Arbeide med iOS VPP-programmer

Les [Slik administrerer du iOS-apper som er kjøpt gjennom et program for volumkjøp, med Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) for å lære om funksjoner, begrensninger og trinn for å gjøre bruk av Apples volumkjøpsprogram og støtte for det i Microsoft Intune.
  
 **Vanlige problemer:** "Jeg tilordnet en iOS VPP-app til brukerne mine, men installasjonen mislyktes."
  
- Dette kan skje hvis ett enkelt VPP-token brukes på tvers av flere leverandører av administrasjon av mobilenheter. VPP-tokener fra Apple kan bare brukes med én leverandør. Hvis du brukte et VPP-token med flere leverandører, må du laste opp tokenet på nytt til Intune.

- Installasjonen kan også mislykkes hvis det totale antallet installasjoner overskrider antall lisenser. Hvis du vil vise en bruksrapport for lisensene dine, går du til siden Lisenser for **Intune-apper-appen.** \> **App licenses** Hvis du vil lære hvordan du tar tilbake lisenser i bruk, kan du se [denne artikkelen.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
