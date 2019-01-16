---
title: Aktivere overvåking av postboks
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28302499"
---
# <a name="enable-mailbox-auditing"></a>Aktivere overvåking av postboks

Hvis du vil aktivere overvåking av postboks for en enkelt bruker eller en hel organisasjon må følgende cmdleter kjøres fra eksterne PowerShell:
  
 **Enkeltbruker**
  
Sett postboks - identitet "Janne Dow" - AuditEnabled $true
  
 **Organisasjon**
  
Get-postboks - ResultSize ubegrenset - filtrere {RecipientTypeDetails - eq "UserMailbox"} | Sett postboks - AuditEnabled $true
  
[få mer informasjon](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

