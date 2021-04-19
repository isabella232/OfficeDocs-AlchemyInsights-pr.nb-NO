---
title: Adressering av påloggingsfeil i Teams AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821996"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Adressering av påloggingsfeil i Teams AADSTS9000411

Når du logger på Microsoft Teams, kan du få feilmeldingen: Beklager, men vi har problemer med å logge deg på **AADSTS9000411: Forespørselen er ikke riktig formatert. Parameteren "login_hint" er duplisert.**

For å løse dette problemet må du sørge for at Microsoft Teams-klientene er oppdatert. Hvis du vil ha mer informasjon om hvordan du oppdaterer klienten, kan [du se Oppdatere Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Hvis du av en eller annen grunn ikke kan oppdatere klienten, vil logging av klienten fjerne de fleste bufrede data. Men hvis du fremdeles har problemer etter avlogging/pålogging, avslutter du Teams og tømmer klienthurtigbufferen ved å gjøre følgende:
1. Lukk Microsoft Teams.
2. Gå til: %appdata%\microsoft\teams, og slett alle filene.
3. Åpne Microsoft Teams på nytt.
