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
# <a name="cdn-used-for-video-playback"></a>CDN brukt til videoavspilling

Live-hendelser fra Stream og eksterne apper, eller live-hendelser fra Yammer/Teams vil automatisk bruke Azure CDN. On-demand videoer som er lastet opp til Stream bruker ikke Azure CDN for avspilling ennå. Videoer som ikke er direkte avspilling spilles av fra Azure Media Services opprinnelsesserver, som er knyttet til tenanten din, i din geografiske region. Hvis du vil ha mer informasjon, kan du se:

- [CDN brukt til videoavspilling](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)
