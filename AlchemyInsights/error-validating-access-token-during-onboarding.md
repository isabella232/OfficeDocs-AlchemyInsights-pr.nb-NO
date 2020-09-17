---
title: Det oppstod en feil under Valide ring av tilgangstoken under skrive bords analyse på kort
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783560"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Feil meldingen «det oppstod en feil under Valide ring av tilgangstoken» under innebygd skrive bords analyse

Denne feilen observeres vanligvis når godkjennings-tokenet utløper. Vanligvis oppdateres tokenet når du oppdaterer siden. Dette problemet kan imidlertid vedvarer hvis det er noen policyer for betinget tilgang som gjelder for kontoen som brukes til lokal skrive bords analyse. Du kan se gjennom loggene av Azure AD-pålogging i Azure-portalen for å se om det finnes påloggings feil for kontoen som brukes til lokal skrive bords analyse.

Hvis du vil ha mer informasjon om betinget tilgang, kan du gå til [planlegge betinget tilgang-distribusjon](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).