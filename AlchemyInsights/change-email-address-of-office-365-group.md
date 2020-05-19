---
title: Endre e-postadressen til en Microsoft 365-gruppe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282929"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>Endre e-postadressen til en Microsoft 365-gruppe

Du kan endre e-postadressen til en Microsoft 365-gruppe ved hjelp av administrasjonssenteret. Bare velg gruppen og velg @edit e-postadresse.

Du kan også bruke følgende EXO PowerShell-kommandoen til å endre den primære SMTP-adressen til en Microsoft 365-gruppe:

Angi UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Eksempel:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
