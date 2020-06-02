---
title: Aktivere overvåking av postboks
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 2bcfb7cc174cd58b21e1bb0c82f0d7cdb25e2fdd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506963"
---
# <a name="enable-mailbox-auditing"></a>Aktivere overvåking av postboks

Hvis du vil aktivere overvåking av postboks for én enkelt bruker eller en hel organisasjon, må følgende cmdleter kjøres fra eksternt strømskall:
  
 **Én bruker**
  
Set-Postboks -Identitet "Jane Dow" -AuditEnabled $true
  
 **Organisasjon**
  
Get-Postboks -ResultSize Ubegrenset -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-mailbox -AuditEnabled $true
  
[få mer informasjon](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

