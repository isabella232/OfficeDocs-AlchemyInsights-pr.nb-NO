---
title: 'Feil: Reglene på denne datamaskinen samsvarer ikke'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981122"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Feil: Reglene på denne datamaskinen samsvarer ikke

Hvis du vil se oppdatert status for dette kjente problemet, kan du se Reglene på denne datamaskinen samsvarer ikke [med reglene på Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Teamet Outlook implementert en løsning i bygg 12928.10000. Løsningen er allerede hos Insider Fast og går til Månedskanal i slutten av juni 2020. Når du har det faste bygget, kan du få meldingen «Hvilke regler vil du beholde» en siste gang. Velg Server når du blir bedt om det, og gå deretter tilbake Outlook og aktiver eventuelle regler som ble deaktivert, på nytt.

Inntil løsningen er tilgjengelig, kan du bruke følgende midlertidig løsning:

**Løsning:** I nylige rapporter har problemet oppstått for de som bare har opprettet klientregler i Outlook skrivebord. Hvis du fortsatt har problemer, kan du vurdere å slette reglene og deretter opprette og redigere regler bare i OWA (Outlook Web App) til problemet er løst.

Hvis du ikke kan slette reglene manuelt, kan du kjøre en Outlook-kommando når du starter Outlook ved å kjøre Outlook.exe /cleanrules. Dette sletter både klient- og serverreglene. Den sletter alle reglene for alle kontoene i Outlook profilen. Denne kommandoen er ytterligere dokumentert i artikkelen Kommandolinjebrytere.

