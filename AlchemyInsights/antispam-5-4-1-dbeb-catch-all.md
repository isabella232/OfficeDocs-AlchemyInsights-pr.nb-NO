---
title: AntiSpam 5.4.1 DBEB fange-alle
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964247"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="219c8-102">Løs leveringsproblemer for feilkode 550 5.4.1 Relay tilgang avslått</span><span class="sxs-lookup"><span data-stu-id="219c8-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="219c8-103">Dette problemet oppstår når du [kontrollerer om en e-postadresse er gyldig for å forhindre bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) når du angir Office 365-nettverket.</span><span class="sxs-lookup"><span data-stu-id="219c8-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="219c8-104">Prøv følgende:</span><span class="sxs-lookup"><span data-stu-id="219c8-104">Try the following:</span></span>

1. <span data-ttu-id="219c8-105">Finn ut om problemet er spesifikt for et helt domene eller en enkelt e-postadresse:</span><span class="sxs-lookup"><span data-stu-id="219c8-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="219c8-106">Hele domenet: noen ganger må domenet synkroniseres. Prøv [å sette domenet til intern og deretter tilbake til autoritativ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="219c8-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
     - <span data-ttu-id="219c8-107">Enkelt e-postadresse: noen ganger må adressen være synkronisert; skiftende det SMTP proxy henvende seg og så skiftende den rygg kanne hjelpe.</span><span class="sxs-lookup"><span data-stu-id="219c8-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="219c8-108">Finn ut om problemet er spesifikt for en gruppe eller fellesmappe.</span><span class="sxs-lookup"><span data-stu-id="219c8-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="219c8-109">For noen objekttyper kan det hende at objektene må opprettes manuelt i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="219c8-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="219c8-110">Hvis du trenger mer hjelp, kan du åpne en støtte billett og angi omfanget av problemet (includidng typen objekt du sender til), slik at vi kan hjelpe deg bedre.</span><span class="sxs-lookup"><span data-stu-id="219c8-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>