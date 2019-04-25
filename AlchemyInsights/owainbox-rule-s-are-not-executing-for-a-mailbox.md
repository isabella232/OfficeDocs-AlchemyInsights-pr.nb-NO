---
title: 1332 OWA - innboks-regler ikke utføres for en bestemt postboks
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32372569"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="1b7c1-102">En regel som ikke virker som forventet</span><span class="sxs-lookup"><span data-stu-id="1b7c1-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="1b7c1-103">Kontroller følgende innstillinger:</span><span class="sxs-lookup"><span data-stu-id="1b7c1-103">Verify the following settings:</span></span>

- <span data-ttu-id="1b7c1-104">En melding kan omadresseres videresendte og besvarte automatisk basert på innboksregler bare én gang.</span><span class="sxs-lookup"><span data-stu-id="1b7c1-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="1b7c1-105">En omadresserer regel (en Innboksregel eller flyt-post, også kjent som regel en transport) kan legge til opptil ti videresending mottakere på en melding.</span><span class="sxs-lookup"><span data-stu-id="1b7c1-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="1b7c1-106">Hvis du vil ha mer informasjon, kan du se [Journal, Transport, og innboksen grenser](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="1b7c1-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="1b7c1-107">Innboksregler fungerer ikke på alternative loggføring postboksen.</span><span class="sxs-lookup"><span data-stu-id="1b7c1-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="1b7c1-108">Hvis du vil ha mer informasjon om alternative loggføring postboksen, kan du se [alternative loggføring postboks](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="1b7c1-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="1b7c1-109">Hvis du vil løse disse problemene, kan du se [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="1b7c1-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="1b7c1-110">Hvis de ovenstående problemene ikke bruker, kjører du innboksen regelen diagnoserapporten før du eskalere problemet til Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="1b7c1-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="1b7c1-111">Åpne postboksen i Outlook på weben, og klikk **Innstillinger** \> **Alternativer** \> **Ordne e-post** \> **innboksregler**.</span><span class="sxs-lookup"><span data-stu-id="1b7c1-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="1b7c1-112">Nederst på siden, klikker du **Hvis reglene ikke virker på Klikk her for å generere en rapport**.</span><span class="sxs-lookup"><span data-stu-id="1b7c1-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
