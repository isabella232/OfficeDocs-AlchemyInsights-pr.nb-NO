---
title: Avsender mottar ikke e-post sendt til Microsoft 365-gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871998"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Avsender mottar ikke e-post sendt til Microsoft 365-gruppe

Som standard mottar ikke avsenderen av en e-postmelding til en Microsoft 365-gruppe en kopi av meldingen i innboksen, selv om avsenderen er medlem av gruppen.

Bruk denne EXO PowerShell-kommandoen til å tillate at avsenderen mottar en kopi av hver e-post de sender til Microsoft 365-gruppen:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Slik aktiverer du innstillingen for alle post bokser samtidig:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Obs!** Endringer i denne innstillingen bruker opptil en time for å få effekt.