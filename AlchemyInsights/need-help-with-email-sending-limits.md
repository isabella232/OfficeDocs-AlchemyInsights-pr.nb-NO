---
title: Trenger du hjelp med sendingsgrenser for e-post?
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
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836288"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="6bcc5-102">Trenger du hjelp med sendingsgrenser for e-post?</span><span class="sxs-lookup"><span data-stu-id="6bcc5-102">Need help with email sending limits?</span></span>

<span data-ttu-id="6bcc5-103">Nedenfor finner **du grensene for sending av by-design** som er håndhevet i tjenesten.</span><span class="sxs-lookup"><span data-stu-id="6bcc5-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="6bcc5-104">Mer informasjon om disse grensene er [dokumentert her](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="6bcc5-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="6bcc5-105">Hvis du vil fraråde levering av uoppfordrede massemeldinger, bruker vi satsegrenser per bruker på alle **utgående og interne meldinger.**</span><span class="sxs-lookup"><span data-stu-id="6bcc5-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="6bcc5-106">På tvers av alle SKUs er denne grensen **10 000 mottakere per dag.**</span><span class="sxs-lookup"><span data-stu-id="6bcc5-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="6bcc5-107">Kunder som trenger å sende legitime masseutsendelser av kommersiell e-post (for eksempel kundenyhetsbrev), bør bruke tredjepartsleverandører som er spesialister på disse tjenestene.</span><span class="sxs-lookup"><span data-stu-id="6bcc5-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="6bcc5-108">**Obs!** Når grensen for mottakerfrekvens er nådd, kan ikke meldinger sendes fra postboksen før antall mottakere som ble sendt meldinger i løpet av de siste 24 timene, faller under grensen.</span><span class="sxs-lookup"><span data-stu-id="6bcc5-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="6bcc5-109">Brukeren kan ikke sende meldinger før dette tidspunktet.</span><span class="sxs-lookup"><span data-stu-id="6bcc5-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="6bcc5-110">Grensen for meldingsfrekvens **på 30 meldinger per minutt** brukes på tvers av alle SKUs.</span><span class="sxs-lookup"><span data-stu-id="6bcc5-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="6bcc5-111">Dette bestemmer hvor mange meldinger en bruker kan sende fra Exchange Online-kontoen i løpet av en angitt periode.</span><span class="sxs-lookup"><span data-stu-id="6bcc5-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="6bcc5-112">Maksimalt antall mottakere som er tillatt i Feltene **Til,** Kopi og Blindkopi for én enkelt e-postmelding, på tvers av alle SKUs, er **1000 mottakere.**</span><span class="sxs-lookup"><span data-stu-id="6bcc5-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="6bcc5-113">Hvis du vil tilpasse denne grensen, kan du [gå hit](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="6bcc5-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
