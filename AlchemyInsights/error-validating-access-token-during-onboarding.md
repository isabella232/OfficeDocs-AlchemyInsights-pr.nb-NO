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
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="f34de-102">Feilmeldingen «Det oppstod en feil under validering av tilgangstoken» under pålasting av skrivebordsanalyse</span><span class="sxs-lookup"><span data-stu-id="f34de-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="f34de-103">Denne feilen er vanligvis observert når godkjenningstokenet utløper.</span><span class="sxs-lookup"><span data-stu-id="f34de-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="f34de-104">Når du oppdaterer siden, oppdateres vanligvis tokenet.</span><span class="sxs-lookup"><span data-stu-id="f34de-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="f34de-105">Dette problemet kan imidlertid vedvare hvis det er noen policyer for betinget tilgang som brukes på kontoen som brukes til innebygd skrivebordsanalyse.</span><span class="sxs-lookup"><span data-stu-id="f34de-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="f34de-106">Du kan se gjennom påloggingsloggene for Azure AD i Azure Portal for å se om det er noen påloggingsfeil for kontoen som brukes for desktop Analytics-introduksjon.</span><span class="sxs-lookup"><span data-stu-id="f34de-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="f34de-107">Hvis du vil ha mer informasjon om betinget tilgang, kan [du gå til Planlegge distribusjon av betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="f34de-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>