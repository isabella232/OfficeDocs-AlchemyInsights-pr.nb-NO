---
title: 'Feil: reglene på denne data maskinen Sams varer ikke'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690972"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Feil: reglene på denne data maskinen Sams varer ikke

Hvis du vil se oppdatert status for dette kjente problemet, kan du se [reglene på denne data maskinen Sams varer ikke med reglene for Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Outlook-teamet har implementert en løsning i bygg 12928,10000. Løsningen er allerede på Insider fast, og vil gå til måneds kanal i den seneste juni 2020. Når du har den faste versjonen, kan du få spørsmål om at du vil beholde "hvilke regler vil du ha" en siste gang. Velg server når du blir bedt om det, og gå deretter tilbake i Outlook, og Aktiver eventuelle regler som ble deaktivert, på nytt.

Følg denne midlertidige løsningen til løsningen er tilgjengelig:

**Løsning**: i nylig brukte rapporter har det oppstått et problem for de som bare har opprettet klient regler i skrive bords versjonen av Outlook. Hvis du fortsetter å kjøre i problemet, bør du vurdere å slette reglene og deretter opprette og redigere regler bare i OWA (Outlook Web App) til problemet er løst.

Hvis du ikke kan slette reglene manuelt, kan du kjøre en Outlook-kommando når du starter Outlook ved å kjøre Outlook.exe/Cleanrules. Dette vil slette både klient-og server reglene. Det vil slette alle reglene for alle kontoene i Outlook-profilen. Denne kommandoen er mer dokumentert i artikkelen bytter mellom kommando linjen.

