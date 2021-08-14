---
title: Endre e-postadressen til en Microsoft 365 gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930738"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Endre e-postadressen til en Microsoft 365 gruppe

Du kan endre e-postadressen til en Microsoft 365 ved hjelp av administrasjonssenteret. Bare velg gruppen, og velg @edit e-postadresse.

Du kan også bruke kommandoen EXO PowerShell til å endre den primære SMTP-adressen til en Microsoft 365 gruppe:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Eksempel:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
