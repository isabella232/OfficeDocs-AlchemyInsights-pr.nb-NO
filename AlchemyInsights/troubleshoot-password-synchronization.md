---
title: Feilsøke synkronisering av passord
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732519"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="e81ea-102">Feilsøke synkronisering av passord</span><span class="sxs-lookup"><span data-stu-id="e81ea-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="e81ea-103">Slik feilsøker du problemer der ingen passord synkroniseres med Azure AD Connect versjon 1.1.614.0 eller senere:</span><span class="sxs-lookup"><span data-stu-id="e81ea-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="e81ea-104">Åpne en ny Windows PowerShell-økt på Azure AD Connect-serveren med alternativet **Kjør som administrator.**</span><span class="sxs-lookup"><span data-stu-id="e81ea-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="e81ea-105">Kjør **Set-ExecutionPolicy RemoteSigned** eller **Set-ExecutionPolicy ubegrenset**.</span><span class="sxs-lookup"><span data-stu-id="e81ea-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="e81ea-106">Start veiviseren for AD-tilkobling for Azure.</span><span class="sxs-lookup"><span data-stu-id="e81ea-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="e81ea-107">Gå til **Flere oppgaver-siden,** velg **Feilsøking**, og klikk **Neste**.</span><span class="sxs-lookup"><span data-stu-id="e81ea-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="e81ea-108">Klikk Start på feilsøking-siden **for å starte feilsøkingsmenyen** i PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e81ea-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="e81ea-109">Velg **Feilsøk synkronisering av passord i**hovedmenyen.</span><span class="sxs-lookup"><span data-stu-id="e81ea-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="e81ea-110">Velg Synkronisering av **passord fungerer ikke i**det hele tatt .</span><span class="sxs-lookup"><span data-stu-id="e81ea-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="e81ea-111">**Forstå resultatene av feilsøkingsoppgaven**</span><span class="sxs-lookup"><span data-stu-id="e81ea-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="e81ea-112">Feilsøkingsoppgaven utfører følgende kontroller:</span><span class="sxs-lookup"><span data-stu-id="e81ea-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="e81ea-113">Validerer at funksjonen for synkronisering av passord er aktivert for Azure AD-leieren.</span><span class="sxs-lookup"><span data-stu-id="e81ea-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="e81ea-114">Validerer at Azure AD Connect-serveren ikke er i oppsamlingsmodus.</span><span class="sxs-lookup"><span data-stu-id="e81ea-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="e81ea-115">For hver eksisterende lokale Active Directory-kobling (som tilsvarer en eksisterende Active Directory-skog):</span><span class="sxs-lookup"><span data-stu-id="e81ea-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="e81ea-116">Validerer at funksjonen for synkronisering av passord er aktivert.</span><span class="sxs-lookup"><span data-stu-id="e81ea-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="e81ea-117">Søker etter hjerterytmehendelser for synkronisering av passord i hendelsesloggene for Windows-programmet.</span><span class="sxs-lookup"><span data-stu-id="e81ea-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="e81ea-118">For hvert Active Directory-domene under den lokale Active Directory-koblingen:</span><span class="sxs-lookup"><span data-stu-id="e81ea-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="e81ea-119">Validerer at domenet kan nås fra Azure AD Connect-serveren.</span><span class="sxs-lookup"><span data-stu-id="e81ea-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="e81ea-120">Validerer at Active Directory Domain Services (AD DS)-kontoer som brukes av den lokale Active Directory-koblingen, har riktig brukernavn, passord og tillatelser som kreves for synkronisering av passord.</span><span class="sxs-lookup"><span data-stu-id="e81ea-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="e81ea-121">Hvis du vil ha mer hjelp til å feilsøke passordsynkronisering, kan du se [Feilsøke synkronisering av passord med Azure AD Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="e81ea-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  