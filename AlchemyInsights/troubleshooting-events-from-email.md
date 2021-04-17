---
title: Feilsøke hendelser fra e-post
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834848"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="b6fd6-102">Feilsøke hendelser fra e-post</span><span class="sxs-lookup"><span data-stu-id="b6fd6-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="b6fd6-103">Kontroller at funksjonen er aktivert for postboksen: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="b6fd6-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="b6fd6-104">Se deretter loggene «Hendelser fra **e-post» Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="b6fd6-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="b6fd6-105">Finn InternetMessageId som samsvarer med elementet i postboksen, i loggene Hendelser fra e-post.</span><span class="sxs-lookup"><span data-stu-id="b6fd6-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="b6fd6-106">TrustScore bestemmer om elementet er lagt til eller ikke.</span><span class="sxs-lookup"><span data-stu-id="b6fd6-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="b6fd6-107">Hendelser legges bare til hvis TrustScore = "Klarert".</span><span class="sxs-lookup"><span data-stu-id="b6fd6-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="b6fd6-108">TrustScore bestemmes av SPF-, Dkim- eller Dmarc-egenskapene, som er i meldingshodet.</span><span class="sxs-lookup"><span data-stu-id="b6fd6-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="b6fd6-109">Slik viser du disse egenskapene:</span><span class="sxs-lookup"><span data-stu-id="b6fd6-109">To view these properties:</span></span>

<span data-ttu-id="b6fd6-110">**Skrivebordsversjonen av Outlook**</span><span class="sxs-lookup"><span data-stu-id="b6fd6-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="b6fd6-111">Åpne elementet</span><span class="sxs-lookup"><span data-stu-id="b6fd6-111">Open the item</span></span>
- <span data-ttu-id="b6fd6-112">Fil -> -> Internett-meldingshoder</span><span class="sxs-lookup"><span data-stu-id="b6fd6-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="b6fd6-113">eller</span><span class="sxs-lookup"><span data-stu-id="b6fd6-113">or</span></span>

<span data-ttu-id="b6fd6-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="b6fd6-114">**MFCMapi**</span></span>

- <span data-ttu-id="b6fd6-115">Gå til elementet i innboksen</span><span class="sxs-lookup"><span data-stu-id="b6fd6-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="b6fd6-116">Se etter PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="b6fd6-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="b6fd6-117">Disse egenskapene bestemmes og registreres under transport og ruting.</span><span class="sxs-lookup"><span data-stu-id="b6fd6-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="b6fd6-118">Hvis du vil ha mer feilsøking, må du kanskje følge opp med transportstøtte om feil i SPF, DKIM og.or DMARC.</span><span class="sxs-lookup"><span data-stu-id="b6fd6-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>