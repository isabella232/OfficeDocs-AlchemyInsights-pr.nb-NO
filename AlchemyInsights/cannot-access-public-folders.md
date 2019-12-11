---
title: Får ikke tilgang til fellesmapper
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959503"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="a664c-102">Outlook kan ikke koble til fellesmapper</span><span class="sxs-lookup"><span data-stu-id="a664c-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="a664c-103">Hvis fellesmappe tilgang ikke fungerer for noen brukere, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="a664c-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="a664c-104">Koble til EXO PowerShell, og Konfigurer DefaultPublicFolderMailbox på problem brukerkontoen slik at den samsvarer med en på en brukerkonto som fungerer.</span><span class="sxs-lookup"><span data-stu-id="a664c-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="a664c-105">Eksempel:</span><span class="sxs-lookup"><span data-stu-id="a664c-105">Example:</span></span>

<span data-ttu-id="a664c-106">Get-postboks WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="a664c-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="a664c-107">Sett postboks ProblemUser-DefaultPublicFolderMailbox \<verdi fra forrige kommando></span><span class="sxs-lookup"><span data-stu-id="a664c-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="a664c-108">Vent minst en time for at endringen skal tre i kraft.</span><span class="sxs-lookup"><span data-stu-id="a664c-108">Wait at least one hour for the change to take effect.</span></span>