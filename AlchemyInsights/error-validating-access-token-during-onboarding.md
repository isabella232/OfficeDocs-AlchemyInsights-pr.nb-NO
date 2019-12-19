---
title: Det oppstod en feil under validering av tilgangs token feil under Desktop Analytics på-boarding
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741232"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>"Det oppstod en feil under validering av tokenet" feil under registreringen av desktop Analytics

Denne feilen er vanligvis observert når godkjenning tokenet utløper. Vanligvis oppdatere siden oppdateres tokenet. Dette problemet kan imidlertid vedvare hvis det er noen policyer for betinget tilgang som brukes på kontoen som brukes til om bord desktop Analytics. Du kan se gjennom loggene for Azure AD Sign in i Azure-portalen for å finne ut om det er noen påloggingsfeil for kontoen som brukes til innføring i desktop Analytics.

Hvis du vil ha mer informasjon om betinget tilgang, kan du gå til [planlegge distribusjonen av betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).