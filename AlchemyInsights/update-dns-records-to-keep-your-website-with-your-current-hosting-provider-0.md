---
title: Oppdater DNS-poster for å beholde nettstedet hos gjeldende vert
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a1ea0589def4945da64c73d68b2e4a3d64d6b83d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506416"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Oppdater DNS-poster for å beholde nettstedet hos gjeldende vert

1. Velg domenet du bruker for webområdet ditt i listen over domener, på [domener](https://portal.office.com/adminportal/home#/Domains) -siden.

2. Velg **+ Ny egendefinert post** og angi følgende:

  - Angi **A (Adresse)** for **DNS-type**

  - **Vertsnavn eller et Alias**, skriver du inn følgende:**@**

  - Skriv inn den statiske IP-adressen for nettstedet ditt der den driftes for øyeblikket (for eksempel: 172.16.140.1), for **IP-adresse**

    Dette må være en  *statisk*  IP-adresse for nettstedet, ikke en  *dynamisk*  IP-adresse. Undersøk området der nettstedet driftes for å være sikker på at du kan få en statisk IP-adresse for det offentlige nettstedet.

3. Velg **Lagre**.

Du kan i tillegg opprette en CNAME-post som lar kundene finne nettstedet.
  
1. Velg **+ Ny egendefinert post** og angi følgende:

  - Angi **CNAME (Alias)** for **DNS-type**

  - Skriv inn **www** for **Vertsnavn eller alias**

  - Skriv inn det fullt kvalifiserte domenenavnet (FQDN) for nettstedet for **Peker til adresse** (for eksempel: contoso.com).

2. Velg **Lagre**.
