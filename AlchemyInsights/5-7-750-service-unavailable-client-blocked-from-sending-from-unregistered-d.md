---
title: 1048 5.7.750 Tjenesten er ikke tilgjengelig. Klient blokkert fra å sende fra uregistrerte domener
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
ms.openlocfilehash: 5879c5996a28e8e9e61c696c51e7c590d1245ba1
ms.sourcegitcommit: edb9be61ff8c4df2a600f70952f6fa731c2093a9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/04/2021
ms.locfileid: "52774260"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="f48c8-103">5.7.750 Klient blokkert fra å sende fra uregistrert domene</span><span class="sxs-lookup"><span data-stu-id="f48c8-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="f48c8-104">Feilen oppstår når et stort antall meldinger sendes fra domener som ikke er klargjort i leieren (lagt til som godtatte domener og validert).</span><span class="sxs-lookup"><span data-stu-id="f48c8-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="f48c8-105">Hvis du vil unngå denne feilen, kan du bruke en sertifikatbasert e-postflytkobling der sertifikatets domene er et klargjort domene, eller du kan klargjøre alle sendingsdomener.</span><span class="sxs-lookup"><span data-stu-id="f48c8-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>

<span data-ttu-id="f48c8-106">Hvis du vil ha mer informasjon, kan du se Løse problemer med levering av e-post for feilkoder [5.7.700 til 5.7.750 i Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).</span><span class="sxs-lookup"><span data-stu-id="f48c8-106">For more information, see [Fix email delivery issues for error codes 5.7.700 through 5.7.750 in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).</span></span>