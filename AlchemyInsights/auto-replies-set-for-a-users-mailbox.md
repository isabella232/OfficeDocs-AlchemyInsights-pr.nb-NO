---
title: Angi automatiske svar for en postboks
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788891"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Angi automatiske svar for postboksen til en bruker

**Metode 1**

1. Logg på portalen for Microsoft 365.

2. Gå til **Brukere > Aktive brukere** (eller **Grupper > Delte postbokser** dersom du angir dette for en delt postboks).

3. Velg en bruker som har en Microsoft Exchange-postboks.

4. Gå til **E-postinnstillinger > Automatiske svar**i undermenyen til høyre (hvis det er en delt postboks, klikker du bare **Automatiske svar** i undermenyen).

**Metode 2**

1. Logg på Microsoft 365-administratorportalen med legitimasjon for administrator. 

2. Velg **Administrasjonssentre**, og klikk deretter på **Exchange**.

3. Klikk på bildet oppe i høyre hjørne, klikk **Annen bruker**, og velg deretter den brukerpostboksen som du vil endre.

4. Velg **Alternativer** på venstre side, klikk på **Organiser e-post**, og klikk deretter på **Automatiske svar.**

**Metode 3**

Kjør følgende cmdlet i Exchange Online PowerShell:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Hvis du vil ha mer informasjon om denne cmdleten, kan du se [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
