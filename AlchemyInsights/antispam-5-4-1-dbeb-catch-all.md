---
title: AntiSpam 5.4.1 DBEB catch-all
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
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707920"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="404f8-102">Løs leveringsproblemer for feilkode 550 5.4.1 Relétilgang nektet</span><span class="sxs-lookup"><span data-stu-id="404f8-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="404f8-103">Dette problemet oppstår når [du kontrollerer om en e-postadresse er gyldig for å hindre tilbakeslag](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) når du går inn i Microsoft-nettverket.</span><span class="sxs-lookup"><span data-stu-id="404f8-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="404f8-104">Prøv følgende:</span><span class="sxs-lookup"><span data-stu-id="404f8-104">Try the following:</span></span>

1. <span data-ttu-id="404f8-105">Finn ut om problemet er spesifikt for et helt domene eller en enkelt e-postadresse:</span><span class="sxs-lookup"><span data-stu-id="404f8-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="404f8-106">Hele domenet: Noen ganger må domenet synkroniseres. prøve [å sette domenet til Intern og deretter tilbake til Autoritativ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="404f8-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="404f8-107">Én e-postadresse: Noen ganger må adressen synkroniseres. endre smtp proxy-adressen og deretter endre den tilbake kan hjelpe.</span><span class="sxs-lookup"><span data-stu-id="404f8-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="404f8-108">Finn ut om problemet er spesifikt for en gruppe eller fellesmappe.</span><span class="sxs-lookup"><span data-stu-id="404f8-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="404f8-109">For enkelte objekttyper må det hende at objektene opprettes manuelt i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="404f8-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="404f8-110">Hvis du trenger ekstra hjelp, må du åpne en støttebillett og angi omfanget av problemet (inkludert typen objekt du sender til), slik at vi kan hjelpe deg bedre.</span><span class="sxs-lookup"><span data-stu-id="404f8-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>