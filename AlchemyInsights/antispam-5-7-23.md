---
title: Antispam-5.7.23
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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682226"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Løs problemer med e-postlevering for feilkode 5.7.23

Kontroller SPF DNS-posten for domenet på en offentlig tilgjengelig SPF-eller DNS-post-kontroll på weben.

Kontroller at den utgående meldingen ikke ble identifisert som søppelpost av Office 365 og rutet gjennom [høy risiko leverings utvalget](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Meldinger i utvalget for høy risiko levering vil ikke bestå SPF-kontroller, og vil derfor ikke bli godtatt av e-postadressen for målorganisasjonen.

Hvis problemet vedvarer, må du kanskje kontakte administratoren for e-verten du prøver å sende e-post til. Noter den detaljerte eksterne feilen som er tilgjengelig i returmeldingen.  Støtte for Office 365 vil kanskje ikke kunne hjelpe videre.