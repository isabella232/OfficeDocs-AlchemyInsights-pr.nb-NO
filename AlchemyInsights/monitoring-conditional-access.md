---
title: Overvåke betinget tilgang
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: f4153f8a87a138d548c133142b0d48a319bd4b71
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656576"
---
# <a name="monitoring-conditional-access"></a>Overvåke betinget tilgang

Målrettet med betinget tilgang får brukere en e-postmelding med varsel hvis de ikke oppfyller tilgangskravene for din organisasjon. Hvis du vil løse, anbefales det at én eller flere av følgende løsninger:
  
- Hvis enheten er antas å være registrert, råder brukeren til å gå til Company Portal-app, og kontroller at vises det i Company Portal. Hvis ikke, bør du registrere enheten.
    
- Gå til i Azure portalen **Intune \> kompatibilitet for enheten**. Klikk **enheten kompatibilitet**under **skjermen** . Vis enhet-kompatibilitet rapporten til å bekrefte at brukerens enhet er merket som kompatibel. 
    
- Gå til i Azure portalen **Intune \> kompatibilitet for enheten**. Under **Administrer**Klikk **policyer**. Kontroller at det er tilordnet en profil til brukerens enhet i listen over samsvar policyer. Hvis ingen profil er tilordnet, vil deretter Intune ikke kunne bekrefte kompatibilitetsstatus for enheten. 
    
- Redigere tilordningen for brukerens betinget tilgang.
    
1. Gå til i Azure portalen **Intune \> betinget tilgang \> policyer for**
    
2. Velg en policy fra listen
    
3. Velg **brukere og grupper**
    
4. Hvis du vil angi en bestemt policy på en person, kan du legge dem til **listen** . For å sikre at en person er utelatt fra policyen, kan du legge dem til i **Ekskluder** -listen. 
    
Les mer: [Slik skjerm betinget tilgang enheter](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

