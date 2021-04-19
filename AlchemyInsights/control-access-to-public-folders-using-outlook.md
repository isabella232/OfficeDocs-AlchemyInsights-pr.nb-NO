---
title: Kontrollere tilgang til fellesmapper ved hjelp av Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816749"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="b8a7b-102">Kontrollere tilgang til fellesmapper ved hjelp av Outlook</span><span class="sxs-lookup"><span data-stu-id="b8a7b-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="b8a7b-103">Slik kontrollerer du hvilke brukere som har tilgang til fellesmapper ved hjelp av Outlook:</span><span class="sxs-lookup"><span data-stu-id="b8a7b-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="b8a7b-104">Bruk `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="b8a7b-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="b8a7b-105">$true: Gi brukere tilgang til fellesmapper i Outlook</span><span class="sxs-lookup"><span data-stu-id="b8a7b-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="b8a7b-106">$false: Hindre brukertilgang til fellesmapper i Outlook.</span><span class="sxs-lookup"><span data-stu-id="b8a7b-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="b8a7b-107">Dette er standardverdien.</span><span class="sxs-lookup"><span data-stu-id="b8a7b-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="b8a7b-108">Obs! Denne fremgangsmåten kan bare kontrollere tilkoblinger med Skrivebordsversjonen av Outlook for Windows-klienter.</span><span class="sxs-lookup"><span data-stu-id="b8a7b-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="b8a7b-109">Brukere kan fortsette å få tilgang til fellesmapper ved hjelp av OWA eller Outlook for Mac.</span><span class="sxs-lookup"><span data-stu-id="b8a7b-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="b8a7b-110">Hvis du vil ha mer informasjon, kan du se Kontrollerte tilkoblinger til [fellesmapper i Outlook](https://aka.ms/controlpf) hvis du vil ha mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="b8a7b-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
