---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717334"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="3f2fd-102">Løse problemer med levering av e-post for feilkode 5.7.23</span><span class="sxs-lookup"><span data-stu-id="3f2fd-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="3f2fd-103">Kontroller DNS-posten for SPF for domenet ditt på en offentlig tilgjengelig SPF-eller DNS-postkontroll på nettet.</span><span class="sxs-lookup"><span data-stu-id="3f2fd-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="3f2fd-104">Kontroller at den utgående meldingen ikke ble identifisert som søppel post av Microsoft og distribuert gjennom det [leverings utvalget for høy risiko](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="3f2fd-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="3f2fd-105">Meldinger i leverings utvalget for høy risiko sender ikke SPF-kontroller, og kan derfor ikke godtas av mål-e-postorganisasjonen.</span><span class="sxs-lookup"><span data-stu-id="3f2fd-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="3f2fd-106">Hvis problemet vedvarer, må du kanskje kontakte administratoren for e-postvertet som du prøver å sende e-post til.</span><span class="sxs-lookup"><span data-stu-id="3f2fd-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="3f2fd-107">Noter ned den detaljerte eksterne feilen som er tilgjengelig i sprett-meldingen.</span><span class="sxs-lookup"><span data-stu-id="3f2fd-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="3f2fd-108">Microsoft kunde støtte vil kanskje ikke kunne hjelpe deg.</span><span class="sxs-lookup"><span data-stu-id="3f2fd-108">Microsoft support may not be able to assist further.</span></span>
