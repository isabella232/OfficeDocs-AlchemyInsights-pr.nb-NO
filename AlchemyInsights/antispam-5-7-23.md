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
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676506"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Løs problemer med levering av e-post for feilkode 5.7.23

Kontroller SPF DNS-posten for domenet ditt på en offentlig tilgjengelig SPF- eller DNS-postkontrollpå nettet.

Kontroller at den utgående meldingen ikke ble identifisert som søppelpost av Microsoft, og rutet gjennom [leveringsutvalget med høy risiko](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Meldinger i utvalget for levering med høy risiko passerer ikke SPF-kontroller, og vil derfor ikke bli akseptert av destinasjons-e-postorganisasjonen.

Hvis problemet vedvarer, må du kanskje kontakte administratoren for e-postverten du prøver å sende e-post til. Noter deg den detaljerte eksterne feilen som er tilgjengelig i fluktmeldingen. Microsoft-støtte kan kanskje ikke hjelpe ytterligere.
