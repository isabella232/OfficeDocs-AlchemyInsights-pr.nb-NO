---
title: Antispam – 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821420"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Løse problemer med levering av e-post for feilkode 5.7.23

Kontroller SPF DNS-posten for domenet ditt på en offentlig tilgjengelig SPF- eller DNS-postkontroll på nettet.

Kontroller at den utgående meldingen ikke ble identifisert som søppelpost av Microsoft, og rutes gjennom utvalget for levering [med høy risiko.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Meldinger i utvalget for levering med høy risiko vil ikke passere SPF-kontroller, og godtas derfor ikke av mål-e-postorganisasjonen.

Hvis problemet vedvarer, må du kanskje kontakte administratoren for e-postverten du prøver å sende e-post til. Noter den detaljerte eksterne feilen som er tilgjengelig i returmeldingen. Microsoft Kundestøtte kan kanskje ikke hjelpe deg videre.
