---
title: Får ikke tilgang til felles mapper
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
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341412"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="ea3db-102">Outlook kan ikke koble til felles mapper</span><span class="sxs-lookup"><span data-stu-id="ea3db-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="ea3db-103">Hvis tilgang til felles mapper ikke fungerer for enkelte brukere, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="ea3db-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="ea3db-104">Koble deg til EXO PowerShell, og Konfigurer DefaultPublicFolderMailbox-parameteren på problem bruker kontoen for å samsvare med parameteren på en arbeids bruker konto.</span><span class="sxs-lookup"><span data-stu-id="ea3db-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="ea3db-105">Eksempel</span><span class="sxs-lookup"><span data-stu-id="ea3db-105">Example:</span></span>

<span data-ttu-id="ea3db-106">Hent post boks WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="ea3db-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="ea3db-107">Set-post boks ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="ea3db-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="ea3db-108">Vent minst én time før endringen trer i kraft.</span><span class="sxs-lookup"><span data-stu-id="ea3db-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="ea3db-109">Hvis problemet fortsetter, kan du følge [denne Fremgangs måten](https://aka.ms/pfcte) for å feilsøke problemer med tilgang til felles mapper ved hjelp av Outlook.</span><span class="sxs-lookup"><span data-stu-id="ea3db-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="ea3db-110">**Slik styrer du hvilke brukere som har tilgang til felles mapper ved hjelp av Outlook**:</span><span class="sxs-lookup"><span data-stu-id="ea3db-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="ea3db-111">Bruke Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true eller $FALSE</span><span class="sxs-lookup"><span data-stu-id="ea3db-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="ea3db-112">$true: gi brukere tilgang til felles mapper i Outlook</span><span class="sxs-lookup"><span data-stu-id="ea3db-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="ea3db-113">$false: hindre bruker tilgang til felles mapper i Outlook.</span><span class="sxs-lookup"><span data-stu-id="ea3db-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="ea3db-114">Dette er standardverdien.</span><span class="sxs-lookup"><span data-stu-id="ea3db-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="ea3db-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="ea3db-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="ea3db-116">**Obs!** Denne Fremgangs måten kan bare kontrollere tilkoblinger med skrive bords versjonen av Outlook for Windows-klienter.</span><span class="sxs-lookup"><span data-stu-id="ea3db-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="ea3db-117">En bruker kan fortsette å få tilgang til felles mapper ved hjelp av OWA eller Outlook for Mac.</span><span class="sxs-lookup"><span data-stu-id="ea3db-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="ea3db-118">Hvis du vil ha mer informasjon, kan du se [kunngjørings støtte for kontrollerte tilkoblinger til felles mapper i Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="ea3db-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>