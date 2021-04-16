---
title: Det oppstod en feil under validering av tilgangstokenfeil under skrivebordsanalyse ombordstigning
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813697"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Feilmeldingen «Det oppstod en feil under validering av tilgangstoken» under pålasting av skrivebordsanalyse

Denne feilen er vanligvis observert når godkjenningstokenet utløper. Når du oppdaterer siden, oppdateres vanligvis tokenet. Dette problemet kan imidlertid vedvare hvis det er noen policyer for betinget tilgang som brukes på kontoen som brukes til innebygd skrivebordsanalyse. Du kan se gjennom påloggingsloggene for Azure AD i Azure Portal for å se om det er noen påloggingsfeil for kontoen som brukes for desktop Analytics-introduksjon.

Hvis du vil ha mer informasjon om betinget tilgang, kan [du gå til Planlegge distribusjon av betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).