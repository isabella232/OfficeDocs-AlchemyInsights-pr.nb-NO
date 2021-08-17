---
title: Løse regler for avsenderadresse/domeneliste
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
ms.openlocfilehash: db8b921fc84f42b6cef1138dca9ad433e648e0a2f10e80927bd5b0222bfeae3b
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896120"
---
# <a name="fix-sender-addressdomain-list-rules"></a>Løse regler for avsenderadresse/domeneliste

En av policyene for søppelpost påvirket denne meldingen. Avsenderen av meldingen ble funnet i en tillatelses- eller blokkeringsliste. Gjør følgende for å se gjennom policyene:

1. I Microsoft 365 Defender-portalen på går du til Policyer for e-& for samarbeid & policyer for trusler mot søppelpost i <https://security.microsoft.com/>  \>  \>  \>  **Policyer-delen.**

   Hvis du vil gå direkte til **siden for søppelpostpolicyer,** bruker du <https://security.microsoft.com/antispam> .

2. Velg **policyen** ved å klikke på navnet på policyen på siden Policyer for  søppelpost (**Type** er egendefinert **søppelpostpolicy** eller Navnet er inngående policy for søppelpost **(standard).**
3. Velg Rediger tillatte og blokkerte avsendere og domener i tillatte og blokkerte avsendere og **domener-delen** i detaljer-undermenyen som vises. 
4. Se gjennom **avsendere** og domener i Tillatt-delen ved å klikke Behandle **\<nn\> avsendere** eller **Tillat domener**.

Hvis du vil ha mer informasjon, [kan du se Konfigurere søppelpostpolicyer i EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
