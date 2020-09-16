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
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="1d5a6-102">Aktivere logging av post boks</span><span class="sxs-lookup"><span data-stu-id="1d5a6-102">Enable mailbox auditing</span></span>

<span data-ttu-id="1d5a6-103">Hvis du vil aktivere post boks overvåking for en enkelt bruker eller en hel organisasjon, må følgende cmdleter kjøres fra ekstern Power Shell:</span><span class="sxs-lookup"><span data-stu-id="1d5a6-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="1d5a6-104">**Enkelt bruker**</span><span class="sxs-lookup"><span data-stu-id="1d5a6-104">**Single User**</span></span>
  
<span data-ttu-id="1d5a6-105">Set-post boks-identitet "Janne Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="1d5a6-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="1d5a6-106">**Bedrift**</span><span class="sxs-lookup"><span data-stu-id="1d5a6-106">**Organization**</span></span>
  
<span data-ttu-id="1d5a6-107">Get-Mailbox-ResultSize Unlimited-filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-post boks-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="1d5a6-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="1d5a6-108">få mer informasjon</span><span class="sxs-lookup"><span data-stu-id="1d5a6-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

