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
ms.openlocfilehash: 157baa1f1e3f48b47ba07b8c6d446f8e081a4ad24b7d48f50c4fc5af5518cdd6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896084"
---
# <a name="fix-tenant-policy-action-override"></a>Løse tenantpolicy (handlingsoverstyring)

En av policyene for søppelpost påvirket denne meldingen. Gjør følgende for å se gjennom policyene:

1. I Microsoft 365 Defender-portalen på går du til Policyer & e-post for samarbeid & policyer for trusler mot søppelpost i <https://security.microsoft.com/>  \>  \>  \>  **Policyer-delen.**

   Hvis du vil gå direkte til **siden for søppelpostpolicyer,** bruker du <https://security.microsoft.com/antispam> .

2. Velg **policyen** ved å klikke på navnet på policyen på siden Policyer for  søppelpost (**Type** er egendefinert **søppelpostpolicy** eller Navnet er inngående policy for søppelpost **(standard).**
3. Velg Rediger handlinger i Handlinger-delen  i detaljer-undermenyen som vises. 
4.  Se gjennom **dommene** for søppelpost, søppelpost, **phishing** og phishing med høy trygghet under Meldingshandlinger for å se om noen av følgende verdier er valgt: 
   - **Legg til X-topptekst**
   - **Prepend emnelinje med tekst**
   - **Omdiriger melding til e-postadresse**
   - **Slett melding**
   - **Ingen handling**

   Det er mulig at **standardinnstillingene for** alle Exchange Online Protection berørte meldingen.

Hvis du vil ha mer informasjon, [kan du se Konfigurere søppelpostpolicyer i EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
