---
title: Oppbevaringspolicyer i Exchange administrasjonssenteret fungerer ikke
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: c9061fa728edaab6575a7b1027783e56739a6d14
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29935001"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="b97f5-102">Oppbevaringspolicyer i Exchange administrasjonssenteret</span><span class="sxs-lookup"><span data-stu-id="b97f5-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="b97f5-103">**Problem:** Opprettet nylig eller oppdatert oppbevaringspolicyer i administrasjonssenteret Exchange er ikke å bruke på postbokser eller varer ikke flyttes til arkiv-postboks eller slettet.</span><span class="sxs-lookup"><span data-stu-id="b97f5-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="b97f5-104">**Årsaker:**</span><span class="sxs-lookup"><span data-stu-id="b97f5-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="b97f5-p101">Dette kan være fordi den **Administrerte Mappeassistent** ikke behandlet brukerens postboks. Administrerte Mappeassistent prøver å behandle hver postboks i organisasjonen \\\cloud-based én gang hver sjuende dag. Hvis du endrer en kode for oppbevaring, eller bruke en annen oppbevaringspolicy på en postboks, kan du vente til den administrerte mappen hjelpe behandler postboksen, eller du kan kjøre cmdleten Start-ManagedFolderAssistant for å starte administrert Mappeassistent for å behandle en bestemt postboks. Kjøre denne cmdleten er nyttig for testing eller feilsøke en oppbevaringspolicy eller innstillingene for oppbevaring av koden. Hvis du vil ha mer informasjon, kan du gå til [kjører forvaltet Mappeassistent](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="b97f5-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="b97f5-110">**Løsning:** Kjør følgende kommando for å starte administrert Mappeassistent for en bestemt postboks:</span><span class="sxs-lookup"><span data-stu-id="b97f5-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="b97f5-p102">Dette kan også være skje hvis **RetentionHold** er **aktivert** for postboksen. Hvis postboksen er plassert i en RetentionHold, behandles ikke oppbevaringspolicy på postboksen i løpet av denne tiden. For mer dataarkiveringsløsninger på RetentionHold innstillingen se: [Postboks oppbevaring Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="b97f5-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="b97f5-114">**Løsning:**</span><span class="sxs-lookup"><span data-stu-id="b97f5-114">**Solution:**</span></span>
    
  - <span data-ttu-id="b97f5-115">Kontrollere statusen for RetentionHold-innstillingen i den bestemte postboksen i [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="b97f5-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="b97f5-116">Kjør følgende kommando for å **deaktivere** RetentionHold på en bestemt postboks:</span><span class="sxs-lookup"><span data-stu-id="b97f5-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="b97f5-117">Nå, kjøre den administrerte mappen hjelperen på nytt:</span><span class="sxs-lookup"><span data-stu-id="b97f5-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="b97f5-118">**Merk:** Hvis en postboks er mindre enn 10 MB, behandler administrert Mappeassistent automatisk ikke postboksen.</span><span class="sxs-lookup"><span data-stu-id="b97f5-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

