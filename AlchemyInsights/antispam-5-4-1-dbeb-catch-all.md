---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821456"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="339f1-102">Løse leveringsproblemer for feilkode 550 5.4.1 Videresendingstilgang nektet</span><span class="sxs-lookup"><span data-stu-id="339f1-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="339f1-103">Dette problemet oppstår når [du kontrollerer om en e-postadresse er](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) gyldig for å forhindre returmeldinger når du går inn i Microsoft-nettverket.</span><span class="sxs-lookup"><span data-stu-id="339f1-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="339f1-104">Prøv følgende:</span><span class="sxs-lookup"><span data-stu-id="339f1-104">Try the following:</span></span>

1. <span data-ttu-id="339f1-105">Finn ut om problemet er spesifikt for et helt domene eller én enkelt e-postadresse:</span><span class="sxs-lookup"><span data-stu-id="339f1-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="339f1-106">Hele domenet: Noen ganger må domenet synkroniseres. prøv [å sette domenet til Internt, og deretter tilbake til Autoritativ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="339f1-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="339f1-107">Enkel e-postadresse: Noen ganger må adressen synkroniseres. Det kan hjelpe å endre smtp-proxy-adressen og deretter endre den tilbake.</span><span class="sxs-lookup"><span data-stu-id="339f1-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="339f1-108">Finn ut om problemet er spesifikt for en gruppe eller fellesmappe.</span><span class="sxs-lookup"><span data-stu-id="339f1-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="339f1-109">For enkelte objekttyper kan det hende at objektene må opprettes manuelt i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="339f1-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="339f1-110">Hvis du trenger mer hjelp, kan du åpne en støtteforespørsel og angi omfanget av problemet (inkludert objekttypen du sender til), slik at vi kan hjelpe deg bedre.</span><span class="sxs-lookup"><span data-stu-id="339f1-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>