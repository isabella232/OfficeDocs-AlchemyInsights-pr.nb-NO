---
title: Antispam – 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821420"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="3bd43-102">Løse problemer med levering av e-post for feilkode 5.7.23</span><span class="sxs-lookup"><span data-stu-id="3bd43-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="3bd43-103">Kontroller SPF DNS-posten for domenet ditt på en offentlig tilgjengelig SPF- eller DNS-postkontroll på nettet.</span><span class="sxs-lookup"><span data-stu-id="3bd43-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="3bd43-104">Kontroller at den utgående meldingen ikke ble identifisert som søppelpost av Microsoft, og rutes gjennom utvalget for levering [med høy risiko.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="3bd43-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="3bd43-105">Meldinger i utvalget for levering med høy risiko vil ikke passere SPF-kontroller, og godtas derfor ikke av mål-e-postorganisasjonen.</span><span class="sxs-lookup"><span data-stu-id="3bd43-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="3bd43-106">Hvis problemet vedvarer, må du kanskje kontakte administratoren for e-postverten du prøver å sende e-post til.</span><span class="sxs-lookup"><span data-stu-id="3bd43-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="3bd43-107">Noter den detaljerte eksterne feilen som er tilgjengelig i returmeldingen.</span><span class="sxs-lookup"><span data-stu-id="3bd43-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="3bd43-108">Microsoft Kundestøtte kan kanskje ikke hjelpe deg videre.</span><span class="sxs-lookup"><span data-stu-id="3bd43-108">Microsoft support may not be able to assist further.</span></span>
