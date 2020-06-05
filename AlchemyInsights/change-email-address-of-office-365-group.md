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
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580666"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Endre e-postadressen til en Microsoft 365-gruppe

Du kan endre e-postadressen til en Microsoft 365-gruppe ved hjelp av administrasjonssenteret. Bare velg gruppen og velg @edit e-postadresse.

Du kan også bruke følgende EXO PowerShell -kommandoen til å endre den primære SMTP-adressen til en Microsoft 365-gruppe:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Eksempel:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
