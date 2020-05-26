---
title: Løse teams påloggingsfeil AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357875"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Løse teams påloggingsfeil AADSTS9000411

Når du logger på Microsoft Teams, kan du få feilmeldingen: **Beklager, men vi har problemer med å logge deg på AADSTS9000411: Forespørselen er ikke riktig formatert. Parameteren "login_hint" dupliseres.**

Hvis du vil løse dette problemet, må du kontrollere at Microsoft Teams-klientene dine er oppdatert. Hvis du vil ha mer informasjon om hvordan du oppdaterer klienten, kan du se [Oppdatere Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Hvis du av en eller annen grunn ikke kan oppdatere klienten, fjerner du de fleste hurtigbufrede dataene når du logger av klienten. Hvis du fortsatt har problemer etter avlogging/pålogging, avslutter du Teams og fjerner klientbufferen ved å gjøre følgende:
1. Lukk Microsoft Teams.
2. Gå til: %appdata%\microsoft\teams, og slett alle filene.
3. Åpne Microsoft Teams på nytt.
