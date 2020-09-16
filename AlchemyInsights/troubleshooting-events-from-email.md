---
title: Feilsøke hendelser fra e-post
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658743"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="31422-102">Feilsøke hendelser fra e-post</span><span class="sxs-lookup"><span data-stu-id="31422-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="31422-103">Kontroller at funksjonen er aktivert for post boksen: \*\*Get-EventsFromEmailConfiguration-Identity <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="31422-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="31422-104">Se deretter på hendelser fra e-postloggene **Eksporter-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="31422-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="31422-105">Finn InternetMessageId som Sams varer med elementet i post boksen, i hendelsene fra e-post-loggene.</span><span class="sxs-lookup"><span data-stu-id="31422-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="31422-106">TrustScore bestemmer om elementet skal legges til eller ikke.</span><span class="sxs-lookup"><span data-stu-id="31422-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="31422-107">Hendelser blir bare lagt til hvis TrustScore = «klarert».</span><span class="sxs-lookup"><span data-stu-id="31422-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="31422-108">TrustScore bestemmes av SPF-, DKIM-eller dMarc-egenskapene, som er i meldings hodet.</span><span class="sxs-lookup"><span data-stu-id="31422-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="31422-109">Slik viser du disse egenskapene:</span><span class="sxs-lookup"><span data-stu-id="31422-109">To view these properties:</span></span>

<span data-ttu-id="31422-110">**Skrive bords Outlook**</span><span class="sxs-lookup"><span data-stu-id="31422-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="31422-111">Åpne elementet</span><span class="sxs-lookup"><span data-stu-id="31422-111">Open the item</span></span>
- <span data-ttu-id="31422-112">Fil – > egenskaper – > Internett-meldingshoder</span><span class="sxs-lookup"><span data-stu-id="31422-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="31422-113">eller</span><span class="sxs-lookup"><span data-stu-id="31422-113">or</span></span>

<span data-ttu-id="31422-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="31422-114">**MFCMapi**</span></span>

- <span data-ttu-id="31422-115">Navigere til elementet i innboksen</span><span class="sxs-lookup"><span data-stu-id="31422-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="31422-116">Se etter PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="31422-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="31422-117">Disse egenskapene bestemmes og registreres under transport og ruting.</span><span class="sxs-lookup"><span data-stu-id="31422-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="31422-118">For videre feil søking må du kanskje følge opp med transport støtte om feilene i SPF, DKIM og. eller DMARC.</span><span class="sxs-lookup"><span data-stu-id="31422-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>