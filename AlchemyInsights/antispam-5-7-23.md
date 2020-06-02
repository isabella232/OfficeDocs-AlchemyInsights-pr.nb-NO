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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506452"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="23727-102">Løs problemer med levering av e-post for feilkode 5.7.23</span><span class="sxs-lookup"><span data-stu-id="23727-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="23727-103">Kontroller SPF DNS-posten for domenet ditt på en offentlig tilgjengelig SPF- eller DNS-postkontroll på nettet.</span><span class="sxs-lookup"><span data-stu-id="23727-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="23727-104">Kontroller at den utgående meldingen ikke ble identifisert som spam av Microsoft og rutet gjennom [utvalget for levering av høy risiko](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="23727-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="23727-105">Meldinger i utvalget for levering med høy risiko vil ikke bestå SPF-kontroller, og godtas derfor ikke av destinasjons-e-postorganisasjonen.</span><span class="sxs-lookup"><span data-stu-id="23727-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="23727-106">Hvis problemet vedvarer, må du kanskje kontakte administratoren for e-postverten du prøver å sende e-post til.</span><span class="sxs-lookup"><span data-stu-id="23727-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="23727-107">Legg merke til den detaljerte eksterne feilen som er tilgjengelig i returmeldingen.</span><span class="sxs-lookup"><span data-stu-id="23727-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="23727-108">Microsoft-støtte kan kanskje ikke hjelpe ytterligere.</span><span class="sxs-lookup"><span data-stu-id="23727-108">Microsoft support may not be able to assist further.</span></span>
