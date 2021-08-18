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
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326806"
---
# <a name="fix-tenant-policy-action-override"></a>Løse tenantpolicy (handlingsoverstyring)

En av policyene for søppelpost påvirket denne meldingen. Gjør følgende for å se gjennom policyene:

1. I Microsoft 365 Defender-portalen på går du til Policyer & for e-post & policyer for trusler mot søppelpost i <https://security.microsoft.com/>  \>  \>  \> **policyer-delen.** 

   Hvis du vil gå direkte til **siden for søppelpostpolicyer,** bruker du <https://security.microsoft.com/antispam> .

2. Velg **policyen** ved å klikke på navnet på policyen på siden Policyer for  søppelpost (**Type** er egendefinert **søppelpostpolicy** eller Navnet er inngående policy for søppelpost **(standard).**
3. Velg Rediger handlinger i Handlinger-delen  i detaljer-undermenyen som vises. 
4.  Se gjennom **dommene** for søppelpost, søppelpost, **phishing** og phishing med høy trygghet under Meldingshandlinger for å se om noen av følgende verdier er valgt: 
   - **Legg til X-topptekst**
   - **Prepend emnelinje med tekst**
   - **Omdiriger melding til e-postadresse**
   - **Slett melding**
   - **Ingen handling**

   Det er mulig at **standardinnstillingene som** ble brukt på alle Exchange Online Protection kunder, påvirket meldingen.

Hvis du vil ha mer informasjon, [kan du se Konfigurere søppelpostpolicyer i EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
