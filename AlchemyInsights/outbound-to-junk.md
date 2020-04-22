---
title: Utgående e-post til søppelpostmappen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 2350586e95f316061ff855d152e86db0547eb209
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761177"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="e6640-102">Utgående e-post til søppelpostmappen</span><span class="sxs-lookup"><span data-stu-id="e6640-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="e6640-103">Hvis du ser utgående meldinger som merkes som søppelpost, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="e6640-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="e6640-104">Hvis du ikke allerede har gjort det, kan du vurdere [å konfigurere varsler om utgående spampolicy](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="e6640-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="e6640-105">Bruk [meldingssporing](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) for å se om den utgående meldingen har **søppelpostverdien for** hendelsesverdien med flere detaljer: **Bruk leveringsutvalg med høy risiko**.</span><span class="sxs-lookup"><span data-stu-id="e6640-105">Use [message trace](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="e6640-106">For disse meldingene kan du se meldingsinnholdet for å se hva som kan betraktes som søppelpost.</span><span class="sxs-lookup"><span data-stu-id="e6640-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="e6640-107">Signaturer kan for eksempel noen ganger forårsake problemer for mange brukere.</span><span class="sxs-lookup"><span data-stu-id="e6640-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="e6640-108">Hvis du har flere eksempler på legitime utgående meldinger som merkes som søppelpost, åpner du en støttebillett og ber støtteagenten om å sende inn meldingene dine som falske positiver til våre spamanalytikere.</span><span class="sxs-lookup"><span data-stu-id="e6640-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="e6640-109">Vær forberedt på å gi eksempelmeldinger som inneholder alle meldingshoder.</span><span class="sxs-lookup"><span data-stu-id="e6640-109">Be prepared to provide sample messages that include all message headers.</span></span>
