---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717334"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Løse problemer med levering av e-post for feilkode 5.7.23

Kontroller DNS-posten for SPF for domenet ditt på en offentlig tilgjengelig SPF-eller DNS-postkontroll på nettet.

Kontroller at den utgående meldingen ikke ble identifisert som søppel post av Microsoft og distribuert gjennom det [leverings utvalget for høy risiko](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Meldinger i leverings utvalget for høy risiko sender ikke SPF-kontroller, og kan derfor ikke godtas av mål-e-postorganisasjonen.

Hvis problemet vedvarer, må du kanskje kontakte administratoren for e-postvertet som du prøver å sende e-post til. Noter ned den detaljerte eksterne feilen som er tilgjengelig i sprett-meldingen. Microsoft kunde støtte vil kanskje ikke kunne hjelpe deg.
