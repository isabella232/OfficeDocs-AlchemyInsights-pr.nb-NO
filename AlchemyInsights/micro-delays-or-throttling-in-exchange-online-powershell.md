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
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702135"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro-forsinkelser eller -begrensning i Exchange Online PowerShell

Du kan se «Micro-forsinkelse i bruk»-advarsler eller forsinkelser når du kjører skript og cmdleter i Exchange Online. Her er noen forslag til hvordan du løser dette:

- Kjør diagnosen vår for å slappe av leierens PowerShell-begrensningspolicyer. Denne løsningen løser problemet for de fleste.
- Hvis problemet fremdeles ikke er løst, kan [du bruke Exchange Online v2 PowerShell-modulen](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), som inneholder CMDleter som er basert på REST API og er betydelig mer performant. Dette kan være en flott løsning for mange Get-CMDleter som brukes ofte.
- Hvis du trenger å bruke CMDleter som ikke dekkes i v2-modulen, kan du se Kjøre [PowerShell-cmdleter for](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)et stort antall brukere i Office 365 , som snakker om hvordan du kommer deg rundt Begrensninger for PowerShell-begrensning i Exchange Online.
