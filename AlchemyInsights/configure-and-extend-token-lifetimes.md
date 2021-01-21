---
title: Konfigurere og forlenge leve tider for token
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917006"
---
# <a name="configure-and-extend-token-lifetimes"></a>Konfigurere og forlenge leve tider for token

Du kan angi leve tiden til et Access-, SAML-eller ID-token utstedt av Microsoft Identity Platform. Du kan angi token-levetid for alle apper i organisasjonen, for et multi-leier (multi-Organization) program eller for en bestemt tjeneste konto i organisasjonen. Hvis du vil ha mer informasjon, kan du lese [konfigurerbare token-leve tider](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

Eksempler [på hvordan du kan lese eksempler på hvordan du konfigurerer leve tid for token](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Hvis du vil lære hvordan du konfigurerer en leve tid og kompatibilitet for et token i Azure Active Directory-B2C (Azure AD B2C), kan du se [konfigurere tokener i Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

Artikkelen [konfigurere virke måten for økten i Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) beskriver metodene for enkel pålogging (SSO) som brukes i Azure ad B2C, og hjelper deg med å velge den mest riktige SSO-metoden når du konfigurerer policyen.

**Hvor lenge kommer tokener? Hvor lenge er de gyldige for?**

Token-Lifetime er 1 time og øktens leve tid er 24 timer. Dette betyr at hvis det ikke har blitt foretatt noen forespørsler i løpet av 24 timer, må du logge på på nytt før du ber om et nytt token.

> [!NOTE]
> Etter at du har blitt 30, 2020, kan du ikke bruke en ny leier policy for å konfigurere økt-og oppdaterings koder. Avgangen skjer innenfor flere måneder etter dette, noe som betyr at vi slutter å føre til eksisterende økt-og oppdaterings kode policyer. Du kan fortsatt konfigurere leve tiden for tilgangs token etter utløpet.






