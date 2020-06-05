---
title: Feilsøke hendelser fra e-post
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569409"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="da274-102">Feilsøke hendelser fra e-post</span><span class="sxs-lookup"><span data-stu-id="da274-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="da274-103">Kontroller at funksjonen er aktivert for postboksen: \*\*Get-EventsFromEmailConfiguration -Identity <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="da274-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="da274-104">Se deretter på 'Hendelser fra **e-post'-loggene Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="da274-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="da274-105">Finn InternetMessageId som samsvarer med elementet i postboksen i loggene "Hendelser fra e-post".</span><span class="sxs-lookup"><span data-stu-id="da274-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="da274-106">TrustScore bestemmer om varen er lagt til eller ikke.</span><span class="sxs-lookup"><span data-stu-id="da274-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="da274-107">Hendelser legges bare til hvis TrustScore = "Klarert".</span><span class="sxs-lookup"><span data-stu-id="da274-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="da274-108">TrustScore bestemmes av SPF-, Dkim- eller Dmarc-egenskapene, som er i meldingshodet.</span><span class="sxs-lookup"><span data-stu-id="da274-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="da274-109">Slik viser du disse egenskapene:</span><span class="sxs-lookup"><span data-stu-id="da274-109">To view these properties:</span></span>

<span data-ttu-id="da274-110">**Skrivebords-Outlook**</span><span class="sxs-lookup"><span data-stu-id="da274-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="da274-111">Åpne elementet</span><span class="sxs-lookup"><span data-stu-id="da274-111">Open the item</span></span>
- <span data-ttu-id="da274-112">Fil -> Egenskaper -> Internett-overskrifter</span><span class="sxs-lookup"><span data-stu-id="da274-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="da274-113">eller</span><span class="sxs-lookup"><span data-stu-id="da274-113">or</span></span>

<span data-ttu-id="da274-114">**MFCMapi (andre)**</span><span class="sxs-lookup"><span data-stu-id="da274-114">**MFCMapi**</span></span>

- <span data-ttu-id="da274-115">Navigere til elementet i innboksen</span><span class="sxs-lookup"><span data-stu-id="da274-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="da274-116">Se etter PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="da274-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="da274-117">Disse egenskapene bestemmes og registreres under transport og ruting.</span><span class="sxs-lookup"><span data-stu-id="da274-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="da274-118">For ytterligere feilsøking må du kanskje følge opp med transportstøtte om feilene i SPF, DKIM og.eller DMARC.</span><span class="sxs-lookup"><span data-stu-id="da274-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>