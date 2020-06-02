---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506452"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Løs problemer med levering av e-post for feilkode 5.7.23

Kontroller SPF DNS-posten for domenet ditt på en offentlig tilgjengelig SPF- eller DNS-postkontroll på nettet.

Kontroller at den utgående meldingen ikke ble identifisert som spam av Microsoft og rutet gjennom [utvalget for levering av høy risiko](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Meldinger i utvalget for levering med høy risiko vil ikke bestå SPF-kontroller, og godtas derfor ikke av destinasjons-e-postorganisasjonen.

Hvis problemet vedvarer, må du kanskje kontakte administratoren for e-postverten du prøver å sende e-post til. Legg merke til den detaljerte eksterne feilen som er tilgjengelig i returmeldingen. Microsoft-støtte kan kanskje ikke hjelpe ytterligere.
