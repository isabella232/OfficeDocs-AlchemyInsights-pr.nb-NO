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
ms.openlocfilehash: 399be421994437d4cd2df644531334c58d177ec3293e7e379d84cd8326823a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54071125"
---
# <a name="cdn-used-for-video-playback"></a>CDN brukt til videoavspilling

Live-hendelser fra Stream og eksterne apper, eller live-hendelser fra Yammer/Teams vil automatisk bruke Azure CDN. On-demand videoer som er lastet opp til Stream bruker ikke Azure CDN for avspilling ennå. Videoer som ikke er direkte avspilling spilles av fra Azure Media Services opprinnelsesserver, som er knyttet til tenanten din, i din geografiske region. Hvis du vil ha mer informasjon, kan du se:

- [CDN brukt til videoavspilling](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)
