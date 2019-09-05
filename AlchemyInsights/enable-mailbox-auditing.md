---
title: Aktivere overvåking av postbokser
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736262"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="7469e-102">Aktivere overvåking av postbokser</span><span class="sxs-lookup"><span data-stu-id="7469e-102">Enable mailbox auditing</span></span>

<span data-ttu-id="7469e-103">Hvis du vil aktivere postboksovervåking for én enkelt bruker eller en hel organisasjon, må følgende cmdleter kjøres fra Remote Power Shell:</span><span class="sxs-lookup"><span data-stu-id="7469e-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="7469e-104">**Enkelt bruker**</span><span class="sxs-lookup"><span data-stu-id="7469e-104">**Single User**</span></span>
  
<span data-ttu-id="7469e-105">Sett-postkasse-identitet "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="7469e-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="7469e-106">**Organisasjon**</span><span class="sxs-lookup"><span data-stu-id="7469e-106">**Organization**</span></span>
  
<span data-ttu-id="7469e-107">Get-postboks-ResultSize Unlimited-filter {RecipientTypeDetails-EQ "UserMailbox"} | Sett postboks-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="7469e-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="7469e-108">få mer informasjon</span><span class="sxs-lookup"><span data-stu-id="7469e-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

