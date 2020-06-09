---
title: 'Feil: Reglene på denne datamaskinen samsvarer ikke'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664255"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Feil: Reglene på denne datamaskinen samsvarer ikke

Hvis du vil se oppdatert status for dette kjente problemet, kan du se [Reglene på denne datamaskinen samsvarer ikke med reglene for Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Outlook-teamet har implementert en løsning i Build 12928.10000. Løsningen er allerede på Insider Fast og vil gå til Månedlig kanal i slutten av juni 2020. Når du har den faste builden, kan du få meldingen "Hvilke regler vil du beholde" en siste gang. Velg Server når du blir bedt om det, og gå deretter tilbake i Outlook og aktivere alle regler som ble deaktivert på nytt.

Til hurtigreparasjonen er tilgjengelig, bruk følgende løsning:

**Løsning**: Det har oppstått problemet for de som bare har opprettet klientregler i Outlook-skrivebordet i nylige rapporter. Hvis du fortsatt støter på problemet, kan du vurdere å slette reglene og deretter opprette og redigere regler bare i OWA (Outlook Web App) til problemet er løst.

Hvis du ikke kan slette reglene manuelt, kan du kjøre en Outlook-kommando når du starter Outlook ved å kjøre Outlook.exe /cleanrules. Dette sletter både klient- og serverreglene. Det vil slette alle reglene for alle kontoene i Outlook-profilen. Denne kommandoen er ytterligere dokumentert i command-line brytere artikkelen.

