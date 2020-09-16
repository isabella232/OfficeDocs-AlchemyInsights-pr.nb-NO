---
title: Aktivere logging av post boks
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806300"
---
# <a name="enable-mailbox-auditing"></a>Aktivere logging av post boks

Hvis du vil aktivere post boks overvåking for en enkelt bruker eller en hel organisasjon, må følgende cmdleter kjøres fra ekstern Power Shell:
  
 **Enkelt bruker**
  
Set-post boks-identitet "Janne Dow"-AuditEnabled $true
  
 **Bedrift**
  
Get-Mailbox-ResultSize Unlimited-filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-post boks-AuditEnabled $true
  
[få mer informasjon](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

