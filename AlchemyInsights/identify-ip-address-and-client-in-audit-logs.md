---
title: Identifisere IP-adresse og klient i overvåkings logger
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668319"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifisere IP-adresse og klient i overvåkings logger

IP-adressen som tilsvarer en aktivitet av en Microsoft 365-bruker eller-administrator, vises i overvåkings loggene. Klient informasjonen er også logget. Her er Fremgangs måten for å identifisere denne informasjonen

1. Logg på [sikkerhets & samsvars senteret til Microsoft 365](https://protection.office.com/).

2. Gå til **Search**  >  **søke siden for overvåkings Logg** for søk.

   Hvis du er interessert i en bestemt aktivitet, velger du den fra **aktiviteter** -listen. Hvis ikke, blir alle aktiviteter returnert for den valgte brukeren (standard innstilling).

   **Obs**! visse aktiviteter er kanskje ikke tilgjengelige i **aktiviteter** -menyen. disse overvåkings elementene blir imidlertid returnert Hvis **Vis resultater for alle aktiviteter** er valgt (standard innstilling).

3. Angi bruker navnet i **brukere** -feltet, Velg det aktuelle dato intervallet for aktiviteten, og klikk deretter **Søk**.

I resultatene kan du se IP-adressen for denne aktiviteten i Resultater-ruten. Velg overvåkings posten for å se detaljert informasjon i **detaljer** -undermenyen (for eksempel klient, bruker som utførte handlinger osv.).

Hvis du vil ha mer informasjon, kan du se [finne IP-adressen til data maskinen som brukes til å få tilgang til en kompromittert konto](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
