---
title: Overvåke betinget tilgang
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418478"
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
  

