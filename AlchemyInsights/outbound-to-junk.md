---
title: Utgående e-post til søppel post mappen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769192"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="3eca7-102">Utgående e-post til søppel post mappen</span><span class="sxs-lookup"><span data-stu-id="3eca7-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="3eca7-103">Hvis du ser utgående meldinger som blir merket som søppel post, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="3eca7-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="3eca7-104">Hvis du ikke allerede har gjort det, bør du vurdere å [konfigurere policyer for utgående søppel post](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="3eca7-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="3eca7-105">Bruk [meldings sporing](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) til å se om den utgående meldingen har hendelses verdien **søppel post** med tilleggs detaljene: **Bruk høy risiko for leverings utvalg**.</span><span class="sxs-lookup"><span data-stu-id="3eca7-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="3eca7-106">For disse meldingene kontrollerer du meldings innholdet for å se hva som kan anses som søppel post.</span><span class="sxs-lookup"><span data-stu-id="3eca7-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="3eca7-107">Signaturer kan for eksempel noen ganger forårsake problemer for mange brukere.</span><span class="sxs-lookup"><span data-stu-id="3eca7-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="3eca7-108">Hvis du har flere eksempler på legitime utgående meldinger som skal merkes som søppel post, åpner du en kunde støtte billett og ber kunde støtte agenten om å sende meldinger som falske positiver til vår søppel post analytikere.</span><span class="sxs-lookup"><span data-stu-id="3eca7-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="3eca7-109">Vær klar til å gi eksempel meldinger som inneholder alle meldings hodene.</span><span class="sxs-lookup"><span data-stu-id="3eca7-109">Be prepared to provide sample messages that include all message headers.</span></span>
