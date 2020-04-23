---
title: Oppbevaringspolicyer i Administrasjonssenter for Exchange fungerer ikke
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
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742442"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="c00eb-102">Oppbevaringspolicyer i administrasjonssenteret for Exchange</span><span class="sxs-lookup"><span data-stu-id="c00eb-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="c00eb-103">**Problem:** Nylig opprettede eller oppdaterte oppbevaringspolicyer i Administrasjonssenter for Exchange gjelder ikke for postbokser eller elementer flyttes ikke til arkivpostboksen eller slettes.</span><span class="sxs-lookup"><span data-stu-id="c00eb-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="c00eb-104">**Grunnårsaker:**</span><span class="sxs-lookup"><span data-stu-id="c00eb-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="c00eb-105">Dette kan skyldes at **hjelperen for administrerte mapper** ikke har behandlet brukerens postboks.</span><span class="sxs-lookup"><span data-stu-id="c00eb-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="c00eb-106">Hjelperen for administrert mappe prøver å behandle alle postbokser i den skybaserte organisasjonen én gang hver sjuende dag.</span><span class="sxs-lookup"><span data-stu-id="c00eb-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="c00eb-107">Hvis du endrer en oppbevaringskode eller bruker en annen oppbevaringspolicy på en postboks, kan du vente til administrertmappeassisten behandler postboksen, eller du kan kjøre cmdleten Start-ManagedFolderAssistant for å starte administrert mappeassistent for å behandle en bestemt postboks.</span><span class="sxs-lookup"><span data-stu-id="c00eb-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="c00eb-108">Kjøring av denne cmdleten er nyttig for testing eller feilsøking av en oppbevaringspolicy eller innstillinger for oppbevaringskode.</span><span class="sxs-lookup"><span data-stu-id="c00eb-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="c00eb-109">Hvis du vil ha mer informasjon, kan du gå [til Kjør assistenten for administrertmappe](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="c00eb-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="c00eb-110">**Løsning:** Kjør følgende kommando for å starte administrert mappeassistent for en bestemt postboks:</span><span class="sxs-lookup"><span data-stu-id="c00eb-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="c00eb-111">Dette kan også skje hvis **RetentionHold** er **aktivert** i postboksen.</span><span class="sxs-lookup"><span data-stu-id="c00eb-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="c00eb-112">Hvis postboksen er plassert på en OppbevaringHold, behandles ikke oppbevaringspolicyen på postboksen i løpet av den tiden.</span><span class="sxs-lookup"><span data-stu-id="c00eb-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="c00eb-113">Hvis du vil ha mer informasjon om oppbevaringshold-innstillingen, kan du se: [Oppbevaringssperre for postboks](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="c00eb-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="c00eb-114">**Løsning:**</span><span class="sxs-lookup"><span data-stu-id="c00eb-114">**Solution:**</span></span>
    
  - <span data-ttu-id="c00eb-115">Kontroller statusen for RetentionHold-innstillingen på den bestemte postboksen i [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="c00eb-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="c00eb-116">Kjør følgende kommando for å **deaktivere** RetentionHold på en bestemt postboks:</span><span class="sxs-lookup"><span data-stu-id="c00eb-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="c00eb-117">Kjør nå assistenten for administrerte mapper på nytt:</span><span class="sxs-lookup"><span data-stu-id="c00eb-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="c00eb-118">**Merk:** Hvis en postboks er mindre enn 10 MB, behandler ikke hjelperen for administrertmappe automatisk postboksen.</span><span class="sxs-lookup"><span data-stu-id="c00eb-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="c00eb-119">Hvis du vil ha mer informasjon om oppbevaringspolicyer i administrasjonssenteret for Exchange, kan du se:</span><span class="sxs-lookup"><span data-stu-id="c00eb-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="c00eb-120">Oppbevaringskoder og oppbevaringspolicyer</span><span class="sxs-lookup"><span data-stu-id="c00eb-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="c00eb-121">Bruke en oppbevaringspolicy på postbokser</span><span class="sxs-lookup"><span data-stu-id="c00eb-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="c00eb-122">Legge til eller fjerne oppbevaringskoder</span><span class="sxs-lookup"><span data-stu-id="c00eb-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="c00eb-123">Slik identifiserer du typen sperring plassert på en postboks</span><span class="sxs-lookup"><span data-stu-id="c00eb-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
