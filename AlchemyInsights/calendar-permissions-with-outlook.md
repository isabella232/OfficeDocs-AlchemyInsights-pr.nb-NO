---
title: Kalendertillatelser
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862173"
---
# <a name="calendar-permissions"></a>Kalendertillatelser

Brukere kan endre sine egne kalendertillatelser med Outlook på nettet eller andre klienter, men som administrator må du kanskje undersøke også.  
Med Exchange PowerShell-cmdleten vil vise deg tillatelsen på en brukers kalender:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Hvis du vil ha mer informasjon, kan du se følgende:

- [Få mailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Sett mailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Legg til MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Kalendertillatelser brukes i deling av kalendere for å se mer informasjon om deling av en Outlook-kalender, se disse artiklene:

- [Dele en Outlook-kalender med andre](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Dele kalenderen i Outlook på nettet for bedrifter](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Hvis du vil feilsøke kalendertillatelse, kan du bruke verktøyet [Støtte- og gjenopprettingsassistent.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)