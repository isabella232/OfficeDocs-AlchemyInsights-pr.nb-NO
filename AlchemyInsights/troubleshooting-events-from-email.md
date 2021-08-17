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
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105361"
---
# <a name="troubleshooting-events-from-email"></a>Feilsøke hendelser fra e-post

1. Kontroller at funksjonen er aktivert for postboksen: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Se deretter loggene «Hendelser fra **e-post» Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Finn InternetMessageId som samsvarer med elementet i postboksen, i loggene Hendelser fra e-post.  

4. TrustScore bestemmer om elementet er lagt til eller ikke. Hendelser legges bare til hvis TrustScore = "Klarert".

TrustScore bestemmes av SPF-, Dkim- eller Dmarc-egenskapene, som er i meldingshodet.

Slik viser du disse egenskapene:

**Skrivebords Outlook**

- Åpne elementet
- Fil -> -> Internett-meldingshoder

eller

**MFCMapi**

- Gå til elementet i innboksen
- Se etter PR_TRANSPORT_MESSAGE_HEADERS_W

Disse egenskapene bestemmes og registreres under transport og ruting. Hvis du vil ha mer feilsøking, må du kanskje følge opp med transportstøtte om feil i SPF, DKIM og.or DMARC.