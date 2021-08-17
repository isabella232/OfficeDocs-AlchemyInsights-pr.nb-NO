---
title: Løse policy for språk/IP-filter
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
ms.openlocfilehash: 16aa12120034e1f848e62bab151d8e30b251a29e5727f085300d74ca7b49ca52
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896164"
---
# <a name="fix-languageip-filter-policy"></a>Løse policy for språk/IP-filter

En av policyene for søppelpost påvirket denne meldingen. Gjør følgende for å se gjennom policyene:

1. I Microsoft 365 Defender-portalen på går du til Policyer & e-post for samarbeid & policyer for trusler mot søppelpost i <https://security.microsoft.com/>  \>  \>  \>  **Policyer-delen.**

   Hvis du vil gå direkte til **siden for søppelpostpolicyer,** bruker du <https://security.microsoft.com/antispam> .

2. Velg **policyen** ved å klikke på navnet på policyen på siden Policyer for  søppelpost (**Type** er egendefinert **søppelpostpolicy** eller Navnet er inngående policy for søppelpost **(standard).**
3. I detaljer-undermenyen som vises, velger du Rediger terskelen for søppelpost og egenskaper i delen Masseutsendelse av  **e-post & søppelpostegenskaper.**
4. Se gjennom innstillingene Inneholder **bestemte** språk og Fra **disse landene** under Merk som søppelpost. 

Hvis du vil ha mer informasjon, [kan du se Konfigurere søppelpostpolicyer i EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
