---
title: Trenger du hjelp med e-postsendingsgrenser?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357868"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="16470-102">Trenger du hjelp med e-postsendingsgrenser?</span><span class="sxs-lookup"><span data-stu-id="16470-102">Need help with email sending limits?</span></span>

<span data-ttu-id="16470-103">Nedenfor er **by-design sende grenser** håndheves i tjenesten.</span><span class="sxs-lookup"><span data-stu-id="16470-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="16470-104">Mer informasjon om disse grensene er dokumentert [her](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="16470-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="16470-105">For å motvirke levering av uønskede massemeldinger, gjelder vi per bruker **mottaker sats grenser for alle utgående og interne meldinger**.</span><span class="sxs-lookup"><span data-stu-id="16470-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="16470-106">På tvers av alle SKU-er er denne grensen **10 000 mottakere per dag**.</span><span class="sxs-lookup"><span data-stu-id="16470-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="16470-107">Kunder som trenger å sende legitim masse kommersiell e-post (for eksempel kundenyhetsbrev) bør bruke tredjepartsleverandører som spesialiserer seg på disse tjenestene.</span><span class="sxs-lookup"><span data-stu-id="16470-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="16470-108">**Merk:** Når mottakerhastighetsgrensen er nådd, kan ikke meldinger sendes fra postboksen før antall mottakere som ble sendt meldinger i løpet av de siste 24 timene faller under grensen.</span><span class="sxs-lookup"><span data-stu-id="16470-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="16470-109">Brukeren vil ikke kunne sende meldinger før det punktet.</span><span class="sxs-lookup"><span data-stu-id="16470-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="16470-110">Meldingshastighetsgrense på **30 meldinger per minutt** brukes på tvers av alle SKU-er.</span><span class="sxs-lookup"><span data-stu-id="16470-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="16470-111">Dette bestemmer hvor mange meldinger en bruker kan sende fra Exchange Online-kontoen innen en angitt periode.</span><span class="sxs-lookup"><span data-stu-id="16470-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="16470-112">Maksimalt antall mottakere som er tillatt i feltene **Til, Kopi og Blindkopi** for én enkelt e-postmelding på tvers av alle SKU-er, er **1000 mottakere**.</span><span class="sxs-lookup"><span data-stu-id="16470-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="16470-113">Hvis du vil tilpasse denne grensen, kan du gå [hit](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="16470-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
