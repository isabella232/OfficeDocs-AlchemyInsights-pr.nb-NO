---
title: Kalender tillatelser
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748802"
---
# <a name="calendar-permissions"></a>Kalender tillatelser

Brukere kan endre sine egne kalender tillatelser med Outlook på nettet eller andre klienter, men som administrator må du også se nærmere på.  
Med Exchange PowerShell-cmdleten kan du vise deg tillatelsene i en brukers kalender:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Hvis du vil se mer informasjon, kan du se følgende:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Legg til-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Kalender tillatelser brukes i deling av kalendere for å se mer informasjon om hvordan du deler en Outlook-kalender, kan du se disse artiklene:

- [Dele en Outlook-kalender med andre](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Dele kalenderen i Outlook på nettet for bedrifter](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Du kan bruke assistent verktøyet for [støtte og gjenoppretting](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) til å feilsøke kalender tillatelser.