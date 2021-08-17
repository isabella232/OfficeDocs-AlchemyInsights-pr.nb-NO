---
title: Identifisere IP-adresse og klient i overvåkingslogger
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
ms.openlocfilehash: 57a1756787f8297a2a1ab3012b95aaa2f33e6045
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313028"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifisere IP-adresse og klient i overvåkingslogger

IP-adressen som tilsvarer en aktivitet av en Microsoft 365 eller administrator, vises i overvåkingsloggene. Klientinformasjonen logges også. Her er fremgangsmåten for å identifisere slik informasjon

1. Logg på Microsoft 365 [samsvarssenteret](https://protection.office.com/).

2. Gå til **søkesiden**  >  **søk i overvåkingsloggen.**

   Hvis du er interessert i en bestemt aktivitet, velger du den fra **Aktiviteter-listen.** Hvis ikke, returneres alle aktiviteter for den valgte brukeren (standardinnstilling).

   **Obs!** Enkelte aktiviteter er kanskje ikke tilgjengelige i **Aktiviteter-menyen.** Disse overvåkingselementene returneres imidlertid hvis Vis resultater **for alle aktiviteter** er valgt (standardinnstilling).

3. Angi brukernavnet i **Brukere-feltet,** velg det aktuelle datointervallet for aktiviteten, og klikk deretter **Søk**.

I resultatene kan du se IP-adressen for denne aktiviteten i resultatruten. Velg overvåkingsposten for å se detaljert informasjon på **Detaljer-undermenyen** (for eksempel Klient, Bruker som utførte handling osv.).

Hvis du vil ha mer informasjon, kan du se [Finne IP-adressen til datamaskinen som brukes til å få tilgang til en kompromittert konto.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
