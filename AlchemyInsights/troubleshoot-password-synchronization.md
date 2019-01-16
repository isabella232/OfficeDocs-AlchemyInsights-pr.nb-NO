---
title: Feilsøking i forbindelse med synkronisering av passord
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28303329"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="d1fb7-102">Feilsøking i forbindelse med synkronisering av passord</span><span class="sxs-lookup"><span data-stu-id="d1fb7-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="d1fb7-103">Slik feilsøker du problemer der ingen passord er synkronisert med Azure AD koble versjon 1.1.614.0 eller senere:</span><span class="sxs-lookup"><span data-stu-id="d1fb7-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="d1fb7-104">Åpne en ny Windows PowerShell-økt på koble til Azure AD-server med alternativet **Kjør som Administrator** .</span><span class="sxs-lookup"><span data-stu-id="d1fb7-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="d1fb7-105">Kjøre **Set-ExecutionPolicy RemoteSigned** eller **Set-ExecutionPolicy ubegrenset**.</span><span class="sxs-lookup"><span data-stu-id="d1fb7-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="d1fb7-106">Start veiviseren Koble til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d1fb7-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="d1fb7-107">Naviger til den \*\* tilleggsoppgaver \*\* velger \*\* feilsøke \*\*, og klikk **Neste**.</span><span class="sxs-lookup"><span data-stu-id="d1fb7-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="d1fb7-108">Klikk **Start for å starte feilsøking** -menyen i PowerShell på siden feilsøking.</span><span class="sxs-lookup"><span data-stu-id="d1fb7-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="d1fb7-109">Velg **Feilsøking i forbindelse med synkronisering av passord**på hovedmenyen.</span><span class="sxs-lookup"><span data-stu-id="d1fb7-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="d1fb7-110">I sub-menyen velger du **synkronisering av passord fungerer ikke i det hele tatt**.</span><span class="sxs-lookup"><span data-stu-id="d1fb7-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="d1fb7-111">**Forstå resultatet av feilsøkingen oppgaven**</span><span class="sxs-lookup"><span data-stu-id="d1fb7-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="d1fb7-112">Feilsøking oppgaven utfører følgende kontroller:</span><span class="sxs-lookup"><span data-stu-id="d1fb7-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="d1fb7-113">Validerer at funksjonen for synkronisering av passord er aktivert for Azure AD-leier.</span><span class="sxs-lookup"><span data-stu-id="d1fb7-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="d1fb7-114">Validerer at Azure AD koble til serveren ikke er i modus for oppsamling.</span><span class="sxs-lookup"><span data-stu-id="d1fb7-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="d1fb7-115">For hvert eksisterende lokale Active Directory connector (som tilsvarer en eksisterende Active Directory-skog):</span><span class="sxs-lookup"><span data-stu-id="d1fb7-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="d1fb7-116">Validerer at funksjonen for synkronisering av passord er aktivert.</span><span class="sxs-lookup"><span data-stu-id="d1fb7-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="d1fb7-117">Søker etter passord synkroniseringshendelser livstegn i hendelsesloggene for Windows-program.</span><span class="sxs-lookup"><span data-stu-id="d1fb7-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="d1fb7-118">For hver Active Directory-domene under lokale Active Directory connector:</span><span class="sxs-lookup"><span data-stu-id="d1fb7-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="d1fb7-119">Validerer at domenet kan nås fra Azure AD koble til serveren.</span><span class="sxs-lookup"><span data-stu-id="d1fb7-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="d1fb7-120">Validerer at Active Directory Domain Services (AD DS)-kontoer som brukes av den lokale Active Directory connector har riktig brukernavn, passord og tillatelser som kreves for synkronisering av passord.</span><span class="sxs-lookup"><span data-stu-id="d1fb7-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="d1fb7-121">Hvis du vil ha mer hjelp, feilsøking i forbindelse med synkronisering av passord, kan du se [Feilsøking i forbindelse med synkronisering av passord med koble til Azure AD-synkronisering](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="d1fb7-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

