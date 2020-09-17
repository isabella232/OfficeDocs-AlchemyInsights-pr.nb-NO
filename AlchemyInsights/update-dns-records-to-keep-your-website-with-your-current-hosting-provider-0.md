---
title: Oppdater DNS-poster for å beholde nettstedet hos gjeldende vert
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815794"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Oppdater DNS-poster for å beholde nettstedet hos gjeldende vert

1. Gå til siden **Konfigurer**domener i administrasjons senteret for Microsoft 365,  >  [Domains](https://admin.microsoft.com/Adminportal#/Domains) og velg domenet du bruker for nettstedet, i listen over domener.

2. Velg **+ Ny egendefinert post** og angi følgende:

  - Angi **A (Adresse)** for **DNS-type**

  - Skriv inn følgende for **verts navn eller alias**: **@**

  - Skriv inn den statiske IP-adressen for nettstedet ditt der den driftes for øyeblikket (for eksempel: 172.16.140.1), for **IP-adresse**

    Dette må være en  *statisk*  IP-adresse for nettstedet, ikke en  *dynamisk*  IP-adresse. Undersøk området der nettstedet driftes for å være sikker på at du kan få en statisk IP-adresse for det offentlige nettstedet.

3. Velg **Lagre**.

Du kan i tillegg opprette en CNAME-post som lar kundene finne nettstedet.
  
1. Velg **+ Ny egendefinert post** og angi følgende:

  - Angi **CNAME (Alias)** for **DNS-type**

  - Skriv inn **www** for **Vertsnavn eller alias**

  - Skriv inn det fullt kvalifiserte domenenavnet (FQDN) for nettstedet for **Peker til adresse** (for eksempel: contoso.com).

2. Velg **Lagre**.
