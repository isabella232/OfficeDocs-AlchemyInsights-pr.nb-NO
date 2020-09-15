---
title: 1332 OWA-innboks (er) kjøres ikke for en post boks
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721600"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>En regel for innboks fungerer ikke som forventet

Kontroller følgende innstillinger i Outlook på nettet:

- En melding kan bare omadresseres, vide res endes eller besvares automatisk basert på regler for innboksen bare én gang. En omdirigerings regel (en regel for en innboks eller en e-postflyt, også kjent som en transport regel), kan legge til maksimalt ti videresendte mottakere i en melding. Hvis du vil ha mer informasjon, kan du se [begrensningene for logg, transport og regler for innboks](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Regler for innboks fungerer ikke på den alternative Logg førings post boksen. Hvis du vil ha mer informasjon om den alternative Logg førings post boksen, kan du se [alternativ Logg føring](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Hvis du vil løse disse problemene, kan du se [KB 2829319](https://support.microsoft.com/kb/2829319).

Hvis de tidligere problemene ikke gjelder, kan du kjøre rapporten for regler for innboks-diagnose før du eskalerer problemet til Microsoft kunde støtte:

1. Åpne post boksen i Outlook på nettet, og klikk <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Innstillinger**  >  **Vise alle Outlook-innstillinger**  >  **E-post**  >  **Regler**.

2. Nederst på siden klikker **du Hvis reglene ikke fungerer, klikker du her for å generere en diagnose rapport**.
