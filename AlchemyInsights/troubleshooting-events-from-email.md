---
title: Feilsøke hendelser fra e-post
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569409"
---
# <a name="troubleshooting-events-from-email"></a>Feilsøke hendelser fra e-post

1. Kontroller at funksjonen er aktivert for postboksen: **Get-EventsFromEmailConfiguration -Identity <mailbox> **

2. Se deretter på 'Hendelser fra **e-post'-loggene Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Finn InternetMessageId som samsvarer med elementet i postboksen i loggene "Hendelser fra e-post".  

4. TrustScore bestemmer om varen er lagt til eller ikke. Hendelser legges bare til hvis TrustScore = "Klarert".

TrustScore bestemmes av SPF-, Dkim- eller Dmarc-egenskapene, som er i meldingshodet.

Slik viser du disse egenskapene:

**Skrivebords-Outlook**

- Åpne elementet
- Fil -> Egenskaper -> Internett-overskrifter

eller

**MFCMapi (andre)**

- Navigere til elementet i innboksen
- Se etter PR_TRANSPORT_MESSAGE_HEADERS_W

Disse egenskapene bestemmes og registreres under transport og ruting. For ytterligere feilsøking må du kanskje følge opp med transportstøtte om feilene i SPF, DKIM og.eller DMARC.