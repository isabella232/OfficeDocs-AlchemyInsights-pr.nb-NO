---
title: Endre e-postadressen til en Microsoft 365-gruppe eller Microsoft Teams
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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819089"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Endre e-postadressen til en Microsoft 365-gruppe eller Microsoft Teams

Du kan endre e-postadressen til en Microsoft 365-gruppe eller Microsoft Teams ved å bruke [Microsoft 365 administrasjonssenter](https://admin.microsoft.com/). Bare velg gruppen, og velg @edit e-postadresse.

Du kan også bruke følgende EXO PowerShell-kommando til å endre den primære SMTP-adressen til en Microsoft 365-gruppe/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Eksempel:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
