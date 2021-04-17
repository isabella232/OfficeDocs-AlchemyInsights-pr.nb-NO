---
title: CDN brukt til videoavspilling
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002552"
- "5146"
ms.openlocfilehash: d9c5f8f586e7f5aa079b28584375516ec8401ca7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819377"
---
# <a name="cdn-used-for-video-playback"></a><span data-ttu-id="d1a39-102">CDN brukt til videoavspilling</span><span class="sxs-lookup"><span data-stu-id="d1a39-102">CDN used for video playback</span></span>

<span data-ttu-id="d1a39-103">Live-hendelser fra Stream og eksterne apper, eller live-hendelser fra Yammer/Teams vil automatisk bruke Azure CDN.</span><span class="sxs-lookup"><span data-stu-id="d1a39-103">Live events from Stream and External app or device live events from Yammer/Teams will automatically use Azure CDN.</span></span> <span data-ttu-id="d1a39-104">On-demand videoer som er lastet opp til Stream bruker ikke Azure CDN for avspilling ennå.</span><span class="sxs-lookup"><span data-stu-id="d1a39-104">On-demand videos uploaded to Stream don't yet use Azure CDN for playback.</span></span> <span data-ttu-id="d1a39-105">Videoer som ikke er direkte avspilling spilles av fra Azure Media Services opprinnelsesserver, som er knyttet til tenanten din, i din geografiske region.</span><span class="sxs-lookup"><span data-stu-id="d1a39-105">Non-live videos in Stream are played back from the Azure Media Services origin server associated with your tenant in your tenant's geographic region.</span></span> <span data-ttu-id="d1a39-106">Hvis du vil ha mer informasjon, kan du se:</span><span class="sxs-lookup"><span data-stu-id="d1a39-106">For more information, see:</span></span>

- [<span data-ttu-id="d1a39-107">CDN brukt til videoavspilling</span><span class="sxs-lookup"><span data-stu-id="d1a39-107">CDN used for video playback</span></span>](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)
