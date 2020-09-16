---
title: Oppbevarings policyer i Exchange admin Center fungerer ikke
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740519"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="6db35-102">Oppbevarings policyer i administrasjons senteret for Exchange</span><span class="sxs-lookup"><span data-stu-id="6db35-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="6db35-103">Hvis du vil at vi skal kjøre automatiske kontroller for innstillingene som nevnes nedenfor, velger du tilbake-knappen < øverst på siden, og deretter skriver du inn e-postadressen til brukeren som har problemer med oppbevarings policyer.</span><span class="sxs-lookup"><span data-stu-id="6db35-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="6db35-104">**Problem:** Nylig opprettede eller oppdaterte oppbevarings policyer i administrasjons senteret for Exchange gjelder ikke for post bokser eller elementer flyttes ikke til arkiv post boksen eller slettes.</span><span class="sxs-lookup"><span data-stu-id="6db35-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="6db35-105">**Hoved årsaker:**</span><span class="sxs-lookup"><span data-stu-id="6db35-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="6db35-106">Dette kan være fordi **assistenten for forvaltede mapper** ikke har behandlet brukerens post boks.</span><span class="sxs-lookup"><span data-stu-id="6db35-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="6db35-107">Den forvaltede mappe assistenten prøver å behandle alle post bokser i en sky BAS ert organisasjon én gang i løpet av sju dager.</span><span class="sxs-lookup"><span data-stu-id="6db35-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="6db35-108">Hvis du endrer en oppbevarings kode eller bruker en annen oppbevarings policy i en post boks, kan du vente til den administrerte mappe assistenten behandler post boksen, eller du kan kjøre Start-ManagedFolderAssistant-cmdleten for å starte en bestemt post boks i den forvaltede mappe.</span><span class="sxs-lookup"><span data-stu-id="6db35-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="6db35-109">Hvis du kjører denne cmdleten, er det nyttig å teste eller feilsøke en oppbevarings kode-innstilling.</span><span class="sxs-lookup"><span data-stu-id="6db35-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="6db35-110">Hvis du vil ha mer informasjon, kan du se [kjøre assistenten for forvaltede mapper](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="6db35-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="6db35-111">**Løsning:** Kjør følgende kommando for å starte den forvaltede mappe assistenten for en bestemt post boks:</span><span class="sxs-lookup"><span data-stu-id="6db35-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="6db35-112">Dette kan også skje hvis **RetentionHold** er **aktivert** på post boksen.</span><span class="sxs-lookup"><span data-stu-id="6db35-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="6db35-113">Hvis post boksen er plassert på en RetentionHold, blir ikke oppbevarings policyen i post boksen behandlet i den perioden.</span><span class="sxs-lookup"><span data-stu-id="6db35-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="6db35-114">Hvis du vil ha mer informasjon på RetentionHold-innstillingen, kan du se: [Oppbevarings plass for post boks](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="6db35-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="6db35-115">**Løsning**</span><span class="sxs-lookup"><span data-stu-id="6db35-115">**Solution:**</span></span>
    
  - <span data-ttu-id="6db35-116">Kontroller statusen for RetentionHold-innstillingen for den bestemte post boksen i [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="6db35-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="6db35-117">Kjør følgende kommando for å **deaktivere** RetentionHold for en bestemt post boks:</span><span class="sxs-lookup"><span data-stu-id="6db35-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="6db35-118">Kjør deretter den administrerte mappe assistenten på nytt:</span><span class="sxs-lookup"><span data-stu-id="6db35-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="6db35-119">**Obs!** Hvis en post boks er mindre enn 10 MB, vil ikke assistenten for forvaltet mappe automatisk behandle post boksen.</span><span class="sxs-lookup"><span data-stu-id="6db35-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="6db35-120">Hvis du vil ha mer informasjon om oppbevarings policyer i administrasjons senteret for Exchange, kan du se:</span><span class="sxs-lookup"><span data-stu-id="6db35-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="6db35-121">Oppbevarings koder og oppbevarings policyer</span><span class="sxs-lookup"><span data-stu-id="6db35-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="6db35-122">Bruke en oppbevarings policy på post bokser</span><span class="sxs-lookup"><span data-stu-id="6db35-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="6db35-123">Legge til eller fjerne oppbevarings koder</span><span class="sxs-lookup"><span data-stu-id="6db35-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="6db35-124">Identifisere hvilken type sperring som skal plasseres i en post boks</span><span class="sxs-lookup"><span data-stu-id="6db35-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
