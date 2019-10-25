---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682226"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="30eba-102">Løs problemer med e-postlevering for feilkode 5.7.23</span><span class="sxs-lookup"><span data-stu-id="30eba-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="30eba-103">Kontroller SPF DNS-posten for domenet på en offentlig tilgjengelig SPF-eller DNS-post-kontroll på weben.</span><span class="sxs-lookup"><span data-stu-id="30eba-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="30eba-104">Kontroller at den utgående meldingen ikke ble identifisert som søppelpost av Office 365 og rutet gjennom [høy risiko leverings utvalget](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="30eba-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="30eba-105">Meldinger i utvalget for høy risiko levering vil ikke bestå SPF-kontroller, og vil derfor ikke bli godtatt av e-postadressen for målorganisasjonen.</span><span class="sxs-lookup"><span data-stu-id="30eba-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="30eba-106">Hvis problemet vedvarer, må du kanskje kontakte administratoren for e-verten du prøver å sende e-post til.</span><span class="sxs-lookup"><span data-stu-id="30eba-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="30eba-107">Noter den detaljerte eksterne feilen som er tilgjengelig i returmeldingen.</span><span class="sxs-lookup"><span data-stu-id="30eba-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="30eba-108">Støtte for Office 365 vil kanskje ikke kunne hjelpe videre.</span><span class="sxs-lookup"><span data-stu-id="30eba-108">Office 365 support may not be able to assist further.</span></span>