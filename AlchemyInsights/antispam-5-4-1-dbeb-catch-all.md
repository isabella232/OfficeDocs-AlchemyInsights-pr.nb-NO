---
title: AntiSpam 5.4.1 DBEB Catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717370"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="fae31-102">Løse leverings problemer for feilkode 550 5.4.1 relé ingen tilgang</span><span class="sxs-lookup"><span data-stu-id="fae31-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="fae31-103">Dette problemet oppstår når [du ser etter at en e-postadresse er gyldig for å forhindre bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) når du skriver inn Microsoft-nettverket.</span><span class="sxs-lookup"><span data-stu-id="fae31-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="fae31-104">Prøv følgende:</span><span class="sxs-lookup"><span data-stu-id="fae31-104">Try the following:</span></span>

1. <span data-ttu-id="fae31-105">Finn ut om problemet er spesifikt for et helt domene eller én enkelt e-post adresse:</span><span class="sxs-lookup"><span data-stu-id="fae31-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="fae31-106">Hele domenet: noen ganger må domenet synkroniseres. Prøv å [Angi domenet til internt, og deretter tilbake til autoritativt](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="fae31-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="fae31-107">Enkel e-post adresse: noen ganger må adressen synkroniseres. å endre SMTP-proxy-adressen og deretter endre den tilbake kan hjelpe deg.</span><span class="sxs-lookup"><span data-stu-id="fae31-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="fae31-108">Finn ut om problemet er spesifikke for en gruppe eller en felles mappe.</span><span class="sxs-lookup"><span data-stu-id="fae31-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="fae31-109">For enkelte objekt typer kan det hende at objektene må opprettes manuelt i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fae31-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="fae31-110">Hvis du trenger mer hjelp, kan du åpne en støtte forespørsel og angi omfanget av problemet (inkludert objekt typen du sender til), slik at vi kan hjelpe deg bedre.</span><span class="sxs-lookup"><span data-stu-id="fae31-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>