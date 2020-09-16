---
title: Feilsøke hendelser fra e-post
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658743"
---
# <a name="troubleshooting-events-from-email"></a>Feilsøke hendelser fra e-post

1. Kontroller at funksjonen er aktivert for post boksen: **Get-EventsFromEmailConfiguration-Identity <mailbox> **

2. Se deretter på hendelser fra e-postloggene **Eksporter-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Finn InternetMessageId som Sams varer med elementet i post boksen, i hendelsene fra e-post-loggene.  

4. TrustScore bestemmer om elementet skal legges til eller ikke. Hendelser blir bare lagt til hvis TrustScore = «klarert».

TrustScore bestemmes av SPF-, DKIM-eller dMarc-egenskapene, som er i meldings hodet.

Slik viser du disse egenskapene:

**Skrive bords Outlook**

- Åpne elementet
- Fil – > egenskaper – > Internett-meldingshoder

eller

**MFCMapi**

- Navigere til elementet i innboksen
- Se etter PR_TRANSPORT_MESSAGE_HEADERS_W

Disse egenskapene bestemmes og registreres under transport og ruting. For videre feil søking må du kanskje følge opp med transport støtte om feilene i SPF, DKIM og. eller DMARC.