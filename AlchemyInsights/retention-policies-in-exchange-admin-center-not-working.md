---
title: Oppbevaringspolicyer i Exchange administrasjonssenter fungerer ikke
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502616"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="e2628-102">Oppbevaringspolicyer i Administrasjonssenter for Exchange</span><span class="sxs-lookup"><span data-stu-id="e2628-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="e2628-103">**Utgave:** Nylig opprettede eller oppdaterte oppbevaringspolicyer i Administrasjonssenter for Exchange gjelder ikke for postbokser eller elementer flyttes ikke til arkivpostboksen eller slettes.</span><span class="sxs-lookup"><span data-stu-id="e2628-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="e2628-104">**Grunnårsaker:**</span><span class="sxs-lookup"><span data-stu-id="e2628-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="e2628-105">Dette kan skyldes **at administrert mappeassistent** ikke har behandlet brukerens postboks.</span><span class="sxs-lookup"><span data-stu-id="e2628-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="e2628-106">Administrert mappeassistent prøver å behandle hver postboks i den skybaserte organisasjonen én gang hver sjuende dag.</span><span class="sxs-lookup"><span data-stu-id="e2628-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="e2628-107">Hvis du endrer en oppbevaringskode eller bruker en annen oppbevaringspolicy på en postboks, kan du vente til administrert mappehjelp behandler postboksen, eller du kan kjøre cmdleten Start-ManagedFolderAssistant for å starte administrertmappeassistent for å behandle en bestemt postboks.</span><span class="sxs-lookup"><span data-stu-id="e2628-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="e2628-108">Hvis du kjører denne cmdleten, kan du prøve eller feilsøke en oppbevaringspolicy eller innstillinger for oppbevaringskode.</span><span class="sxs-lookup"><span data-stu-id="e2628-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="e2628-109">Hvis du vil ha mer informasjon, kan du gå [til Kjør assistenten for administrerte mapper](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="e2628-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="e2628-110">**Løsning:** Kjør følgende kommando for å starte administrert mappeassistent for en bestemt postboks:</span><span class="sxs-lookup"><span data-stu-id="e2628-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="e2628-111">Dette kan også skje hvis **RetentionHold** er **aktivert** på postboksen.</span><span class="sxs-lookup"><span data-stu-id="e2628-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="e2628-112">Hvis postboksen er plassert på en RetentionHoldhold, behandles ikke oppbevaringspolicyen på postboksen i løpet av denne tiden.</span><span class="sxs-lookup"><span data-stu-id="e2628-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="e2628-113">Hvis du vil ha mer informasjon om oppbevaringshold-innstillingen, kan du se Postboks [oppbevaring hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="e2628-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="e2628-114">**Løsning:**</span><span class="sxs-lookup"><span data-stu-id="e2628-114">**Solution:**</span></span>
    
  - <span data-ttu-id="e2628-115">Kontroller statusen for RetentionHoldHold-innstillingen på den bestemte postboksen i [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="e2628-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="e2628-116">Kjør følgende kommando for å **deaktivere** RetentionHold på en bestemt postboks:</span><span class="sxs-lookup"><span data-stu-id="e2628-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="e2628-117">Kjør nå assistenten for administrerte mapper på nytt:</span><span class="sxs-lookup"><span data-stu-id="e2628-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="e2628-118">**Merk:** Hvis en postboks er mindre enn 10 MB, behandler ikke assistenten for administrerte mapper automatisk postboksen.</span><span class="sxs-lookup"><span data-stu-id="e2628-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="e2628-119">Hvis du vil ha mer informasjon om oppbevaringspolicyer i administrasjonssenteret for Exchange, kan du se:</span><span class="sxs-lookup"><span data-stu-id="e2628-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="e2628-120">Oppbevaringskoder og oppbevaringspolicyer</span><span class="sxs-lookup"><span data-stu-id="e2628-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="e2628-121">Bruke en oppbevaringspolicy for postbokser</span><span class="sxs-lookup"><span data-stu-id="e2628-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="e2628-122">Legge til eller fjerne oppbevaringskoder</span><span class="sxs-lookup"><span data-stu-id="e2628-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="e2628-123">Slik identifiserer du typen hold som er plassert på en postboks</span><span class="sxs-lookup"><span data-stu-id="e2628-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
