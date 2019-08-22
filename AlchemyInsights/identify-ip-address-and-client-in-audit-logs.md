---
title: Identifisere IP-adressen og klient i overvåkingslogger
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539038"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifisere IP-adressen og klient i overvåkingslogger

IP-adresse som svarer til en aktivitet med en Office 365-bruker eller administrator vises i overvåkingsloggen. Informasjon om klient logges også. Her er fremgangsmåten for å identifisere slike opplysninger

1. Logg på [Office 365 & kompatibilitet Sikkerhetssenter](https://protection.office.com/).

2. Gå til **Søk** > **Overvåk Logg Søk** -siden.

   Hvis du er interessert i en bestemt aktivitet, kan du velge den fra **aktiviteter** -listen. Hvis ikke, returneres alle aktiviteter for den valgte brukeren (standardinnstilling).

   **Merk**: enkelte aktiviteter er kanskje ikke tilgjengelig i **aktiviteter** -menyen. imidlertid de overvåke varer returneres hvis **Vise resultater for alle aktiviteter som** er valgt (standardinnstillingen).

3. Angi brukernavnet i **brukere** -feltet, velg riktig datointervallet for aktiviteten og deretter **Søk**.

I resultatene, kan du se IP-adressen for denne aktiviteten i resultater-ruten. Velg kontrollregister å se detaljert informasjon i **Detaljer** -undermeny (for eksempel klient, brukeren som utførte handlingen, osv.).

Hvis du vil ha mer informasjon, kan du se [finne IP-adressen til datamaskinen for å få tilgang til et utsatt konto](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
