---
title: Angi automatiske svar for en postboks
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
- "9000761"
- "3514"
ms.openlocfilehash: 85b7e969032607216c948532dcdf83ba09022c7cdfaebce8671c6d2e8fef183d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046617"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Angi automatiske svar for postboksen til en bruker

**Metode 1**

1. Logg på portalen for Microsoft 365.

2. Gå til **Brukere > Aktive brukere** (eller **Grupper > Delte postbokser** dersom du angir dette for en delt postboks).

3. Velg en bruker som har en Microsoft Exchange-postboks.

4. Gå til **E-postinnstillinger > Automatiske svar** i undermenyen til høyre (hvis det er en delt postboks, klikker du bare **Automatiske svar** i undermenyen).

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
