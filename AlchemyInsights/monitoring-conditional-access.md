---
title: Overvåke betinget tilgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702912"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Overvåke betinget tilgang for Exchange

Brukere som er rettet mot betinget tilgang, mottar en e-postvarsling hvis de ikke oppfyller organisasjonens tilgangs krav. Vi anbefaler en eller flere av følgende løsninger for å løse:
  
- Hvis enheten er Presumed for å bli registrert, ber du brukeren om å gå til Firmaportal-appen og kontrollere at den vises i firma portalen. Hvis den ikke gjør det, skal brukeren registrere enheten.
    
- I Azure-portalen går du **til \> enhets samsvar for Intune**. Under **skjerm** Klikk **enhets samsvar**. Vis samsvars rapporten for enheten for å bekrefte at brukerens enhet er merket som kompatibel. 
    
- I Azure-portalen går du **til \> enhets samsvar for Intune**. Klikk **policyer**under **Behandle**. Kontroller at en profil er tilordnet til brukerens enhet i listen over samsvars policyer. Hvis ingen profil er tilordnet, vil ikke Intune kunne bekrefte enhetens samsvars status. 
    
- Rediger brukerens tilordningen for betinget tilgang.
    
1. Gå til **Intune- \> \> policyer for betinget tilgang** i Azure-portalen
    
2. Velg en policy fra listen
    
3. Klikk **brukere og grupper**
    
4. Hvis du vil angi en bestemt policy for noen, kan du legge dem til i **inkluderings** listen. Hvis du vil sikre at en person utelates fra policyen, legger du dem til i **ekskluderings** listen. 
    
Les mer: [Slik overvåker du enheter for betinget tilgang](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

