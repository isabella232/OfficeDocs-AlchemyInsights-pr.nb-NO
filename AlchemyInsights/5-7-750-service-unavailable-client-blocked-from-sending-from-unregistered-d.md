---
title: 1048 5.7.750-tjenesten er ikke tilgjengelig. Klienten blokkert fra å sende fra uregistrerte domener
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 731aa2e155ba3fdaaca7fed9dd51b3e4a3f20f29
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664251"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="fe8cc-103">5.7.750-klient blokkert fra å sende fra uregistrert domene</span><span class="sxs-lookup"><span data-stu-id="fe8cc-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="fe8cc-104">Feilen oppstår når et stort antall meldinger sendes fra domener som ikke er klargjort i leieren (lagt til som godtatte domener og validert).</span><span class="sxs-lookup"><span data-stu-id="fe8cc-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="fe8cc-105">Du kan unngå denne feilen ved å bruke en sertifikat BAS ert e-postflyt der sertifikatets domene er et klargjort domene, eller du kan klargjøre alle sendende domener.</span><span class="sxs-lookup"><span data-stu-id="fe8cc-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
