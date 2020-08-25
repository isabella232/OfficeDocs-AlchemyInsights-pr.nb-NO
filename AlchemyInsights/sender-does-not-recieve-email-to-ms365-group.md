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
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="d9974-102">Avsender mottar ikke e-post sendt til Microsoft 365-gruppe</span><span class="sxs-lookup"><span data-stu-id="d9974-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="d9974-103">Som standard mottar ikke avsenderen av en e-postmelding til en Microsoft 365-gruppe en kopi av meldingen i innboksen, selv om avsenderen er medlem av gruppen.</span><span class="sxs-lookup"><span data-stu-id="d9974-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="d9974-104">Bruk denne EXO PowerShell-kommandoen til å tillate at avsenderen mottar en kopi av hver e-post de sender til Microsoft 365-gruppen:</span><span class="sxs-lookup"><span data-stu-id="d9974-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="d9974-105">Slik aktiverer du innstillingen for alle post bokser samtidig:</span><span class="sxs-lookup"><span data-stu-id="d9974-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="d9974-106">**Obs!** Endringer i denne innstillingen bruker opptil en time for å få effekt.</span><span class="sxs-lookup"><span data-stu-id="d9974-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>