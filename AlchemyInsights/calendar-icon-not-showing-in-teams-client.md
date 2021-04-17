---
title: Kalenderikon som ikke vises i Teams-klienten
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
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819962"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Kalenderikon som ikke vises i Teams-klienten

Kalenderfanen i Teams krever tilgang til en Exchange-postboks via Exchange Web Services. Exchange-postboksen kan være Tilkoblet eller Lokal. For brukere på Internett som ikke kan se Kalenderfanen, må du kontrollere at de [er lisensiert for en Exchange Online-postboks og at postboksen er aktivert](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Hvis brukeren har en gyldig postboks i Exchange Online, men fremdeles ikke kan se kalenderfanen, har du kanskje et nettverks problem. Bruk [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) og Kjør **Microsoft Exchange Web Services (EWS) tilkoblingstester** for den berørte brukeren.

Til slutt sjekker du [Teams-appene – Policyer for appoppsett](https://admin.teams.microsoft.com/policies/app-setup) for å sikre at kalenderappen ikke har blitt fjernet fra policyen som brukes for brukeren (mest sannsynlig er den **Global (organisasjonsomfattende standard)**.

Hvis brukerne dine befinner seg lokalt, må du bekrefte at hybridkonfigurasjonen er OK. Bruk [Veiviseren for hybridkonfigurasjon](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) for å feilsøke.

Vær obs på at [Teams krever Exchange 2016 CU3 eller nyere](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
