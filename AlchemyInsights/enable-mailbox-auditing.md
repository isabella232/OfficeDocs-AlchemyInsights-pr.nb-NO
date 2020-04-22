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
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703580"
---
# <a name="enable-mailbox-auditing"></a>Aktivere overvåking av postboks

Hvis du vil aktivere overvåking av postboks for én enkelt bruker eller en hel organisasjon, må følgende cmdleter kjøres fra Eksternt strømskall:
  
 **Enkelt bruker**
  
Sett-postboks -identitet "Jane Dow" -AuditEnabled $true
  
 **Organisasjon**
  
Get-postboks -ResultSize Ubegrenset -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-postboks -AuditEnabled $true
  
[få mer informasjon](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

