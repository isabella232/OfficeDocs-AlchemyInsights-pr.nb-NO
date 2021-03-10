---
title: Løse tenantpolicy (handlingsoverstyring)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695699"
---
# <a name="fix-tenant-policy-action-override"></a>Løse tenantpolicy (handlingsoverstyring)

En søppelpostpolicy i leieren din påvirket denne meldingen. Hvis du vil se gjennom policyen, gjør du følgende:

1. Gå til sikkerhetssenteret [for Office 365 &,](https://go.microsoft.com/fwlink/p/?linkid=2077143)og gå deretter **til** beskyttelse mot søppelpost for  >    >  [trusselbehandling.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Kontroller om **policykilden** angir følgende:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC-melding**

    Hvis dette er det, **kontrollerer** du innstillingene for policyen som berørte meldingen, på Egendefinert-fanen. Det er mulig at **standardinnstillingene** som brukes for alle Exchange Online Protection-kunder, har påvirket meldingen.

Hvis du vil ha mer informasjon om hvordan du konfigurerer policyer for søppelpostfilteret, kan du [se Konfigurere policyer for søppelpostfilteret.](https://go.microsoft.com/fwlink/?linkid=2101431)
