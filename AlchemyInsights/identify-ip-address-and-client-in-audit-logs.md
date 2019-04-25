---
title: Identifisere IP-adressen og klient i overvåkingslogger
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 7e30a638de5926aa11b8ae637613a48076d7bdc9
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417001"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifisere IP-adressen og klient i overvåkingslogger

IP-adressen som samsvarer med en aktivitet etter en bruker eller administrator vises i overvåkingsloggen. Informasjon om klient logges også. Her er fremgangsmåten for å identifisere slike opplysninger

1. Logg på [Office 365 & kompatibilitet Sikkerhetssenter](https://protection.office.com/)

2. Klikk **Søk og undersøkelser** , og velg **Overvåk Logg Søk**.

   Hvis du er interessert i en bestemt aktivitet, kan du velge den fra **aktiviteter** -listen. Hvis ikke, returneres alle aktiviteter for den valgte brukeren (standardinnstilling).

   **Merk**: enkelte aktiviteter er kanskje ikke tilgjengelig i **aktiviteter** -menyen. imidlertid de overvåke varer returneres hvis **Vise resultater for alle aktiviteter som** er valgt (standardinnstillingen).

3. Angi brukernavnet i **brukere** -feltet, velg riktig datointervallet for aktiviteten og deretter **Søk**.

I resultatene, kan du se IP-adressen for denne aktiviteten i resultater-ruten. Velg kontrollregister å se detaljert informasjon i **Detaljer** -undermeny (for eksempel klient, brukeren som utførte handlingen, osv.).

Hvis du vil ha mer informasjon, kan du se [finne IP-adressen til datamaskinen for å få tilgang til et utsatt konto](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
