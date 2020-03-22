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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891758"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="1bf1e-102">Outlook kan ikke koble til fellesmapper</span><span class="sxs-lookup"><span data-stu-id="1bf1e-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="1bf1e-103">Hvis fellesmappetilgang ikke fungerer for noen brukere, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="1bf1e-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="1bf1e-104">Koble til EXO PowerShell og konfigurer parameteren DefaultPublicFolderMailbox på problembrukerkontoen slik at den samsvarer med parameteren på en fungerende brukerkonto.</span><span class="sxs-lookup"><span data-stu-id="1bf1e-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="1bf1e-105">Eksempel:</span><span class="sxs-lookup"><span data-stu-id="1bf1e-105">Example:</span></span>

<span data-ttu-id="1bf1e-106">Get-Postboks WorkingUser | ft DefaultPublicFolderMailbox, EffektivFellesMappeKasse</span><span class="sxs-lookup"><span data-stu-id="1bf1e-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="1bf1e-107">Set-postboks ProblemUser -DefaultPublicFolderMailbox-verdien \<fra forrige kommando></span><span class="sxs-lookup"><span data-stu-id="1bf1e-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="1bf1e-108">Vent minst en time på at endringen trer i kraft.</span><span class="sxs-lookup"><span data-stu-id="1bf1e-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="1bf1e-109">Hvis problemet forblir, følger du [denne fremgangsmåten](https://aka.ms/pfcte) for å feilsøke tilgangsproblemer for fellesmapper ved hjelp av Outlook.</span><span class="sxs-lookup"><span data-stu-id="1bf1e-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>