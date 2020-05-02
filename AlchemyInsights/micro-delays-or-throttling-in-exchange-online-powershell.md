---
title: Micro-forsinkelser eller -begrensning i Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947905"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro-forsinkelser eller -begrensning i Exchange Online PowerShell

Du kan se «Micro-forsinkelse i bruk»-advarsler eller forsinkelser når du kjører skript og cmdleter i Exchange Online. Her er to forslag relatert til dette:

- Du kan prøve å bruke [Exchange Online v2 PowerShell-modulen](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), som omfatter CMDleter basert på REST API og er betydelig mer velfungerende. Dette kan være en flott løsning for mange Get-CMDleter som brukes ofte.
- Hvis du trenger å bruke CMDleter som ikke dekkes i v2-modulen ennå, kan du se [Kjøre PowerShell-cmdleter for et stort antall brukere i Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), som snakker om hvordan du håndterer forventet PowerShell-begrensning i Exchange Online.
