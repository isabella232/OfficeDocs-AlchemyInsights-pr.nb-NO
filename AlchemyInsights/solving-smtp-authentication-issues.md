---
title: Løse problemer med SMTP-godkjenning
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
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826424"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="3761e-102">Løse problemer med SMTP-godkjenning</span><span class="sxs-lookup"><span data-stu-id="3761e-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="3761e-103">Hvis du får feil 5.7.57 eller 5.7.3 når du prøver å sende SMTP-e-post og godkjenne med en klient eller et program, er det et par ting du bør kontrollere:</span><span class="sxs-lookup"><span data-stu-id="3761e-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="3761e-104">Godkjent SMTP-innsending kan være deaktivert i leieren eller på postboksen du prøver å bruke (kontroller begge innstillingene).</span><span class="sxs-lookup"><span data-stu-id="3761e-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="3761e-105">Hvis du vil lese mer, kan du se [Aktivere eller deaktivere smtp-innsending av godkjent klient.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)</span><span class="sxs-lookup"><span data-stu-id="3761e-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="3761e-106">Kontroller om [Azure-sikkerhetsstandarder](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) er aktivert for leieren. hvis aktivert, vil SMTP-godkjenning ved hjelp av enkel godkjenning (også kjent som eldre, dette bruke brukernavn og passord) mislykkes.</span><span class="sxs-lookup"><span data-stu-id="3761e-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>