---
title: Får ikke tilgang til fellesmapper
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819521"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="0ef36-102">Outlook kan ikke koble til fellesmapper</span><span class="sxs-lookup"><span data-stu-id="0ef36-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="0ef36-103">Hvis tilgang til fellesmapper ikke fungerer for enkelte brukere, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="0ef36-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="0ef36-104">Koble til EXO PowerShell, og konfigurer DefaultPublicFolderMailbox-parameteren på den problematiske brukerkontoen slik at den samsvarer med parameteren på en fungerende brukerkonto.</span><span class="sxs-lookup"><span data-stu-id="0ef36-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="0ef36-105">Eksempel:</span><span class="sxs-lookup"><span data-stu-id="0ef36-105">Example:</span></span>

<span data-ttu-id="0ef36-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="0ef36-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="0ef36-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="0ef36-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="0ef36-108">Vent minst én time før endringen trer i kraft.</span><span class="sxs-lookup"><span data-stu-id="0ef36-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="0ef36-109">Hvis problemet forblir, følger du [denne](https://aka.ms/pfcte) fremgangsmåten for å feilsøke problemer med tilgang til fellesmapper ved hjelp av Outlook.</span><span class="sxs-lookup"><span data-stu-id="0ef36-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="0ef36-110">**Slik kontrollerer du hvilke brukere som har tilgang til fellesmapper ved hjelp av Outlook:**</span><span class="sxs-lookup"><span data-stu-id="0ef36-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="0ef36-111">Bruk Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true eller $false</span><span class="sxs-lookup"><span data-stu-id="0ef36-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="0ef36-112">$true: Gi brukere tilgang til fellesmapper i Outlook</span><span class="sxs-lookup"><span data-stu-id="0ef36-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="0ef36-113">$false: Hindre brukertilgang til fellesmapper i Outlook.</span><span class="sxs-lookup"><span data-stu-id="0ef36-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="0ef36-114">Dette er standardverdien.</span><span class="sxs-lookup"><span data-stu-id="0ef36-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="0ef36-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="0ef36-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="0ef36-116">**Obs!** Denne fremgangsmåten kan bare kontrollere tilkoblinger med Outlook-skrivebord for Windows-klienter.</span><span class="sxs-lookup"><span data-stu-id="0ef36-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="0ef36-117">En bruker kan fortsette å få tilgang til fellesmapper ved hjelp av OWA eller Outlook for Mac.</span><span class="sxs-lookup"><span data-stu-id="0ef36-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="0ef36-118">Hvis du vil ha mer informasjon, kan du [se Annonsere støtte for kontrollerte tilkoblinger til fellesmapper i Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="0ef36-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>