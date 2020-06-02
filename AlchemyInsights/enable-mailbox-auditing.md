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
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="60c24-102">Aktivere overvåking av postboks</span><span class="sxs-lookup"><span data-stu-id="60c24-102">Enable mailbox auditing</span></span>

<span data-ttu-id="60c24-103">Hvis du vil aktivere overvåking av postboks for én enkelt bruker eller en hel organisasjon, må følgende cmdleter kjøres fra eksternt strømskall:</span><span class="sxs-lookup"><span data-stu-id="60c24-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="60c24-104">**Én bruker**</span><span class="sxs-lookup"><span data-stu-id="60c24-104">**Single User**</span></span>
  
<span data-ttu-id="60c24-105">Set-Postboks -Identitet "Jane Dow" -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="60c24-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="60c24-106">**Organisasjon**</span><span class="sxs-lookup"><span data-stu-id="60c24-106">**Organization**</span></span>
  
<span data-ttu-id="60c24-107">Get-Postboks -ResultSize Ubegrenset -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-mailbox -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="60c24-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="60c24-108">få mer informasjon</span><span class="sxs-lookup"><span data-stu-id="60c24-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

