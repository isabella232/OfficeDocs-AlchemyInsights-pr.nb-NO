---
title: Slå på overvåking av postboks
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482473"
---
# <a name="turn-on-mailbox-auditing"></a>Slå på overvåking av postboks

Hvis du vil aktivere overvåking av postboks for én enkelt bruker eller en hel organisasjon, kan du kjøre følgende cmdleter fra ekstern PowerShell:

- **Enkeltbruker:** Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
- **Organisasjon:** Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true

Hvis du vil ha mer informasjon, [kan du se Behandle overvåking av postboks.](https://go.microsoft.com/fwlink/?linkid=2103668)