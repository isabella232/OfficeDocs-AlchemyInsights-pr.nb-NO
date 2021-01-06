---
title: Endre e-postadressen til en Microsoft 365-gruppe eller Microsoft Teams
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
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756566"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Endre e-postadressen til en Microsoft 365-gruppe eller Microsoft Teams

Du kan endre e-postadressen til en Microsoft 365-gruppe eller Microsoft Teams ved å bruke [Microsoft 365 administrasjonssenter](https://admin.microsoft.com/). Bare velg gruppen, og velg @edit e-postadresse.

Du kan også bruke følgende EXO PowerShell-kommando til å endre den primære SMTP-adressen til en Microsoft 365-gruppe/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Eksempel:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
