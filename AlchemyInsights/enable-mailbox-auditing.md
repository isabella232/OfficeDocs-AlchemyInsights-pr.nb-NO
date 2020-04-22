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
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="d6f8f-102">Aktivere overvåking av postboks</span><span class="sxs-lookup"><span data-stu-id="d6f8f-102">Enable mailbox auditing</span></span>

<span data-ttu-id="d6f8f-103">Hvis du vil aktivere overvåking av postboks for én enkelt bruker eller en hel organisasjon, må følgende cmdleter kjøres fra Eksternt strømskall:</span><span class="sxs-lookup"><span data-stu-id="d6f8f-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="d6f8f-104">**Enkelt bruker**</span><span class="sxs-lookup"><span data-stu-id="d6f8f-104">**Single User**</span></span>
  
<span data-ttu-id="d6f8f-105">Sett-postboks -identitet "Jane Dow" -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="d6f8f-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="d6f8f-106">**Organisasjon**</span><span class="sxs-lookup"><span data-stu-id="d6f8f-106">**Organization**</span></span>
  
<span data-ttu-id="d6f8f-107">Get-postboks -ResultSize Ubegrenset -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-postboks -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="d6f8f-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="d6f8f-108">få mer informasjon</span><span class="sxs-lookup"><span data-stu-id="d6f8f-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

