---
title: Oppdater DNS-poster for å beholde nettstedet hos gjeldende vert
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29481726"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Oppdater DNS-poster for å beholde nettstedet hos gjeldende vert

1. Velg domenet du bruker for nettstedet ditt fra listen på [Domener](https://portal.office.com/adminportal/home#/Domains) -siden, og velg deretter **DNS-innstillinger** i administrasjonsruten. 
    
2. Velg **+ Ny egendefinert post** og angi følgende: 
    
  - Angi **A (Adresse)** for **DNS-type**
    
  - Skriv inn @ for **Vertsnavn eller alias**
    
  - Skriv inn den statiske IP-adressen for nettstedet ditt der den driftes for øyeblikket (for eksempel: 172.16.140.1), for **IP-adresse** 
    
    Dette må være en  *statisk*  IP-adresse for nettstedet, ikke en  *dynamisk*  IP-adresse. Undersøk området der nettstedet driftes for å være sikker på at du kan få en statisk IP-adresse for det offentlige nettstedet. 
    
3. Velg **Lagre**. 
    
Du kan i tillegg opprette en CNAME-post som lar kundene finne nettstedet.
  
1. Velg **+ Ny egendefinert post** og angi følgende: 
    
  - Angi **CNAME (Alias)** for **DNS-type**
    
  - Skriv inn **www** for **Vertsnavn eller alias**
    
  - Skriv inn det fullt kvalifiserte domenenavnet (FQDN) for nettstedet for **Peker til adresse** (for eksempel: contoso.com). 
    
2. Velg **Lagre**. 
    

