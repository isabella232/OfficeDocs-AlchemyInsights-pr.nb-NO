---
title: 1336 RecoverableItems-mappen er full
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
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741276"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="c1cfa-102">Mappen gjen opprettelige elementer er full</span><span class="sxs-lookup"><span data-stu-id="c1cfa-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="c1cfa-103">For Exchange Online-postbokser er standard lagrings grense for mappen gjen opprettelige elementer 30 GB.</span><span class="sxs-lookup"><span data-stu-id="c1cfa-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="c1cfa-104">Lagrings grensen for mappen gjen opprettelige elementer økes automatisk til 100 GB hvis post boksen er plassert på en rettslig sperre, i eDiscovery-sperring eller tilordnes til en oppbevarings policy.</span><span class="sxs-lookup"><span data-stu-id="c1cfa-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="c1cfa-105">Når mappen gjen opprettelige elementer når lagrings grensen, påvirkes post boks funksjonaliteten på følgende måter:</span><span class="sxs-lookup"><span data-stu-id="c1cfa-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="c1cfa-106">Brukeren kan ikke slette elementer fra post boksen.</span><span class="sxs-lookup"><span data-stu-id="c1cfa-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="c1cfa-107">Assistenten for forvaltede mapper kan ikke slette elementer basert på oppbevarings kode eller innstillinger for forvaltede mapper.</span><span class="sxs-lookup"><span data-stu-id="c1cfa-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="c1cfa-108">For post bokser som har en enkelt vare gjenoppretting aktivert eller som er satt på vent, kan ikke tillatelse til å opprettholde versjonen av elementer som er redigert av brukeren, bli behandlet.</span><span class="sxs-lookup"><span data-stu-id="c1cfa-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="c1cfa-109">For post bokser der overvåkings logging for post boks er aktivert, kan ikke oppføringer i overvåkings loggen for post boksen lagres i overvåkings under mappen i mappen gjen opprettelige elementer.</span><span class="sxs-lookup"><span data-stu-id="c1cfa-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="c1cfa-110">For post bokser som ikke er på vent, kan administratorer bruke `Search-Mailbox -SearchDumpsterOnly -DeleteContent` kommandoen i Exchange Online PowerShell til å slette elementer i mappen gjen opprettelige elementer.</span><span class="sxs-lookup"><span data-stu-id="c1cfa-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="c1cfa-111">Hvis du vil ha mer informasjon, kan du se følgende emner:</span><span class="sxs-lookup"><span data-stu-id="c1cfa-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="c1cfa-112">Søke etter og slette meldinger</span><span class="sxs-lookup"><span data-stu-id="c1cfa-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="c1cfa-113">Søk – post boks</span><span class="sxs-lookup"><span data-stu-id="c1cfa-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="c1cfa-114">For post bokser som er på vent, må administratorer fjerne sperringen før de kan slette elementer fra mappen gjen opprettelige elementer.</span><span class="sxs-lookup"><span data-stu-id="c1cfa-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="c1cfa-115">Hvis du vil ha mer informasjon, kan du se [slette elementer i mappen gjen opprettelige elementer i Sky BAS ert post bokser på vent](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="c1cfa-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="c1cfa-116">For å hindre at mappen gjen opprettelige elementer blir full, kan administratorer øke lagrings grensen for mappen gjen opprettelige elementer for post bokser på vent og konfigurere en oppbevarings policy for post boks som flytter elementer fra mappen gjen opprettelige elementer til brukerens arkiv post boks.</span><span class="sxs-lookup"><span data-stu-id="c1cfa-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="c1cfa-117">Se [øke gjenopprettende element kvoten for post bokser som er sperret](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="c1cfa-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
