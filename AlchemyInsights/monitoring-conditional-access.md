---
title: Overvåke betinget tilgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713727"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Overvåke betinget tilgang for Exchange

Brukere som er målrettet med betinget tilgang, mottar en e-post om varsler hvis de ikke oppfyller organisasjonens tilgangskrav. For å løse problemet anbefaler vi én eller flere av følgende løsninger:
  
- Hvis enheten antas å være registrert, anbefaler du brukeren å gå til Firmaportal-appen og kontrollerer at den vises i firmaportalen. Hvis den ikke gjør det, bør brukeren registrere enheten.
    
- Gå til **Intune \> Device-samsvar i Azure-portalen.** Klikk **Enhetssamsvar**under **Skjerm.** Vis rapporten om enhetssamsvar for å kontrollere at brukerens enhet er merket som kompatibel. 
    
- Gå til **Intune \> Device-samsvar i Azure-portalen.** Klikk **Policyer**under **Behandle**. Kontroller at en profil er tilordnet brukerens enhet i listen over samsvarspolicyer. Hvis ingen profil er tilordnet, kan ikke Intune bekrefte enhetens samsvarsstatus. 
    
- Rediger brukerens betinget tilgangstilordning.
    
1. Gå til **Intune Betingede tilgangspolicyer \> i Azure-portalen \> **
    
2. Velg en policy fra listen
    
3. Klikk **brukere og grupper**
    
4. Hvis du vil målrette mot en bestemt policy hos noen, legger du dem til i **Inkluder-listen.** Hvis du vil sikre at en person utelates fra policyen, legger du dem til i **Utelat-listen.** 
    
Les mer: [Slik overvåker du enheter med betinget tilgang](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

