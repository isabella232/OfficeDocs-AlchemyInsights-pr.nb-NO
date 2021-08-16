---
title: Micro-forsinkelser eller -begrensning i Exchange Online PowerShell
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
- "3500011"
- "5106"
ms.openlocfilehash: 6753dcb375ea5e19b01c4350b61aa8904aa102112df175a3f70281d18a634dbf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098575"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro-forsinkelser eller -begrensning i Exchange Online PowerShell

Du kan se «Micro-forsinkelse i bruk»-advarsler eller forsinkelser når du kjører skript og cmdleter i Exchange Online. Her er noen forslag til hvordan du løser dette:

- Kjør diagnosen vår for å slappe av leierens PowerShell-begrensningspolicyer. Denne løsningen løser problemet for de fleste.
- Hvis problemet fremdeles ikke er løst, kan [du bruke Exchange Online v2 PowerShell-modulen](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), som inneholder CMDleter som er basert på REST API og er betydelig mer performant. Dette kan være en flott løsning for mange Get-CMDleter som brukes ofte.
- Hvis du trenger å bruke CMDleter som ikke dekkes i v2-modulen, kan du se Kjøre [PowerShell-cmdleter for](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)et stort antall brukere i Office 365 , som snakker om hvordan du kommer deg rundt Begrensninger for PowerShell-begrensning i Exchange Online.
