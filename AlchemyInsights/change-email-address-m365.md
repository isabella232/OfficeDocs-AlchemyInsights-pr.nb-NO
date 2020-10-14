---
title: Endre e-postadressen til Microsoft 365-gruppen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/10/2020
ms.locfileid: "48461946"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Endre e-postadressen til en Microsoft 365-gruppe

Du kan endre e-postadressen til en Microsoft 365-gruppe ved hjelp av administrasjons senteret. Bare Velg gruppen, og velg @edit e-postadresse.

Du kan også bruke EXO PowerShell-kommandoen til å endre den primære SMTP-adressen til en Microsoft 365-gruppe:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Eksempel

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
