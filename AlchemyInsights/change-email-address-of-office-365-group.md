---
title: Endre e-postadressen til en Microsoft 365-gruppe
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
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819053"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Endre e-postadressen til en Microsoft 365-gruppe

Du kan endre e-postadressen til en Microsoft 365-gruppe ved hjelp av administrasjonssenteret. Bare velg gruppen, og velg @edit e-postadresse.

Du kan også bruke kommandoen EXO PowerShell til å endre den primære SMTP-adressen til en Microsoft 365-gruppe:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Eksempel:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
