---
title: Kalender ikonet vises ikke i Microsoft Teams-klienten
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583921"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Kalender ikonet vises ikke i Microsoft Teams-klienten

Kategorien **Kalender** i Teams krever tilgang til en Exchange-postboks via Exchange Web Services. Exchange-postboksen kan være tilkoblet eller lokalt. For brukere på nettet som ikke ser **Kalender** -fanen, må du kontrollere at de [er lisensiert for en Exchange Online-postboks og at post boksen er aktivert](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). Hvis brukerne dine er privat lokalt, må du bekrefte at hybrid konfigurasjonen er OK. Bruk [Veiviseren for hybridkonfigurasjon](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) for å feilsøke. Vær obs på at [Teams krever Exchange 2016 CU3 eller nyere](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Hvis du vil ha mer informasjon og feil søkings trinn, kan du se [Feilsøke problemer med Microsoft Teams og Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).
