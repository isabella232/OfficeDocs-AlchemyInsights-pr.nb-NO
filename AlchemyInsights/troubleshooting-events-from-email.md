---
title: Feilsøke hendelser fra e-post
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834848"
---
# <a name="troubleshooting-events-from-email"></a>Feilsøke hendelser fra e-post

1. Kontroller at funksjonen er aktivert for postboksen: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Se deretter loggene «Hendelser fra **e-post» Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Finn InternetMessageId som samsvarer med elementet i postboksen, i loggene Hendelser fra e-post.  

4. TrustScore bestemmer om elementet er lagt til eller ikke. Hendelser legges bare til hvis TrustScore = "Klarert".

TrustScore bestemmes av SPF-, Dkim- eller Dmarc-egenskapene, som er i meldingshodet.

Slik viser du disse egenskapene:

**Skrivebordsversjonen av Outlook**

- Åpne elementet
- Fil -> -> Internett-meldingshoder

eller

**MFCMapi**

- Gå til elementet i innboksen
- Se etter PR_TRANSPORT_MESSAGE_HEADERS_W

Disse egenskapene bestemmes og registreres under transport og ruting. Hvis du vil ha mer feilsøking, må du kanskje følge opp med transportstøtte om feil i SPF, DKIM og.or DMARC.