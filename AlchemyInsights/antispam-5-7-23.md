---
title: Antispam - 5.7.23
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
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676506"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="f1fbe-102">Løs problemer med levering av e-post for feilkode 5.7.23</span><span class="sxs-lookup"><span data-stu-id="f1fbe-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="f1fbe-103">Kontroller SPF DNS-posten for domenet ditt på en offentlig tilgjengelig SPF- eller DNS-postkontrollpå nettet.</span><span class="sxs-lookup"><span data-stu-id="f1fbe-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="f1fbe-104">Kontroller at den utgående meldingen ikke ble identifisert som søppelpost av Microsoft, og rutet gjennom [leveringsutvalget med høy risiko](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="f1fbe-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="f1fbe-105">Meldinger i utvalget for levering med høy risiko passerer ikke SPF-kontroller, og vil derfor ikke bli akseptert av destinasjons-e-postorganisasjonen.</span><span class="sxs-lookup"><span data-stu-id="f1fbe-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="f1fbe-106">Hvis problemet vedvarer, må du kanskje kontakte administratoren for e-postverten du prøver å sende e-post til.</span><span class="sxs-lookup"><span data-stu-id="f1fbe-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="f1fbe-107">Noter deg den detaljerte eksterne feilen som er tilgjengelig i fluktmeldingen.</span><span class="sxs-lookup"><span data-stu-id="f1fbe-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="f1fbe-108">Microsoft-støtte kan kanskje ikke hjelpe ytterligere.</span><span class="sxs-lookup"><span data-stu-id="f1fbe-108">Microsoft support may not be able to assist further.</span></span>
