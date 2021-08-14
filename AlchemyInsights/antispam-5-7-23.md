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
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932178"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Løse problemer med levering av e-post for feilkode 5.7.23

Kontroller SPF DNS-posten for domenet ditt på en offentlig tilgjengelig SPF- eller DNS-postkontroll på nettet.

Kontroller at den utgående meldingen ikke ble identifisert som søppelpost av Microsoft, og rutes gjennom utvalget for levering [med høy risiko.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Meldinger i utvalget for levering med høy risiko vil ikke passere SPF-kontroller, og godtas derfor ikke av mål-e-postorganisasjonen.

Hvis problemet vedvarer, må du kanskje kontakte administratoren for e-postverten du prøver å sende e-post til. Noter den detaljerte eksterne feilen som er tilgjengelig i returmeldingen. Microsoft Kundestøtte kan kanskje ikke hjelpe deg videre.
