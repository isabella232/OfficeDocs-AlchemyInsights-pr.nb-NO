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
ms.openlocfilehash: 2fab21f76f455815979ae162c1ce8246ad5c297e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314709"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro-forsinkelser eller -begrensning i Exchange Online PowerShell

Du kan se «Micro-forsinkelse i bruk»-advarsler eller forsinkelser når du kjører skript og cmdleter i Exchange Online. Her er noen forslag til hvordan du løser dette:

- Kjør diagnosen vår for å slappe av leierens PowerShell-begrensningspolicyer. Denne løsningen løser problemet for de fleste.
- Hvis problemet fremdeles ikke er løst, [bruker du Exchange Online v2 PowerShell-modulen](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), som inneholder CMDleter som er basert på REST API og er betydelig mer performant. Dette kan være en flott løsning for mange Get-CMDleter som brukes ofte.
- Hvis du trenger å bruke CMDleter som ikke dekkes i v2-modulen, kan du se Kjøre [PowerShell-cmdleter for](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)et stort antall brukere i Office 365 , som snakker om hvordan du kommer deg rundt Begrensninger for PowerShell-begrensning i Exchange Online.
