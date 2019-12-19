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
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="55b2a-102">"Det oppstod en feil under validering av tokenet" feil under registreringen av desktop Analytics</span><span class="sxs-lookup"><span data-stu-id="55b2a-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="55b2a-103">Denne feilen er vanligvis observert når godkjenning tokenet utløper.</span><span class="sxs-lookup"><span data-stu-id="55b2a-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="55b2a-104">Vanligvis oppdatere siden oppdateres tokenet.</span><span class="sxs-lookup"><span data-stu-id="55b2a-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="55b2a-105">Dette problemet kan imidlertid vedvare hvis det er noen policyer for betinget tilgang som brukes på kontoen som brukes til om bord desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="55b2a-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="55b2a-106">Du kan se gjennom loggene for Azure AD Sign in i Azure-portalen for å finne ut om det er noen påloggingsfeil for kontoen som brukes til innføring i desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="55b2a-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="55b2a-107">Hvis du vil ha mer informasjon om betinget tilgang, kan du gå til [planlegge distribusjonen av betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="55b2a-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>