---
title: Identifisere IP-adresse og klient i overvåkingslogger
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716397"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifisere IP-adresse og klient i overvåkingslogger

IP-adressen som tilsvarer en aktivitet av en Microsoft 365-bruker eller administrator, vises i overvåkingsloggene. Klientinformasjonen logges også. Her er fremgangsmåten for å identifisere slik informasjon

1. Logg på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Gå til**søkesiden for søkeloggen for søke etter** søk i **søkesiden for søkeetter søk.** > 

   Hvis du er interessert i en bestemt aktivitet, velger du den fra **Aktivitetsliste.** Hvis ikke, returneres alle aktiviteter for den valgte brukeren (standardinnstilling).

   **Merk:** Enkelte aktiviteter er kanskje ikke tilgjengelige i **Aktiviteter-menyen.** Disse overvåkingselementene returneres imidlertid hvis **Vis resultater for alle aktiviteter** er valgt (standardinnstilling).

3. Angi brukernavnet i **Brukere-feltet,** velg riktig datoperiode for aktiviteten, og klikk deretter **Søk**.

I resultatene kan du se IP-adressen for denne aktiviteten i resultatruten. Velg overvåkingsoppføringen for å se detaljert informasjon i **undermenyen Detaljer** (for eksempel Klient, Bruker som utførte handlingen osv.).

Hvis du vil ha mer informasjon, kan du se [Finne IP-adressen til datamaskinen som brukes til å få tilgang til en kompromittert konto](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
