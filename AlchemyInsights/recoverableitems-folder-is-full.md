---
title: 1336 RecoverableItems mappen er full
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510761"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="23772-102">Mappen Gjenopprettelige elementer er full</span><span class="sxs-lookup"><span data-stu-id="23772-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="23772-103">For Exchange Online-postbokser er standard lagringsgrense for mappen Gjenopprettelige elementer 30 GB.</span><span class="sxs-lookup"><span data-stu-id="23772-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="23772-104">Lagringsgrensen for mappen Gjenopprettelige elementer økes automatisk til 100 GB hvis postboksen er plassert på prosedyresperre, eDiscovery hold eller er tilordnet til en oppbevaringspolicy.</span><span class="sxs-lookup"><span data-stu-id="23772-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="23772-105">Når mappen Gjenopprettelige elementer når lagringsgrensen, påvirkes postboksfunksjonaliteten på følgende måter:</span><span class="sxs-lookup"><span data-stu-id="23772-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="23772-106">Brukeren kan ikke slette elementer fra postboksen.</span><span class="sxs-lookup"><span data-stu-id="23772-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="23772-107">Administrert mappeassistent kan ikke slette elementer basert på lagringskode eller administrerte mappeinnstillinger.</span><span class="sxs-lookup"><span data-stu-id="23772-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="23772-108">For postbokser som har enkel elementgjenoppretting aktivert eller er plassert på vent, kan ikke beskyttelsesprosessen for copy-on-write-siden vedlikeholde versjoner av elementer som er redigert av brukeren.</span><span class="sxs-lookup"><span data-stu-id="23772-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="23772-109">For postbokser som har postboks overvåking logging aktivert, ingen postboks overvåkingsloggoppføringer kan lagres i undermappen overvåkingser i mappen Gjenopprettelige elementer.</span><span class="sxs-lookup"><span data-stu-id="23772-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="23772-110">For postbokser som ikke er på vent, kan administratorer bruke `Search-Mailbox -SearchDumpsterOnly -DeleteContent` kommandoen i Exchange Online PowerShell til å slette elementer i mappen Gjenopprettelige elementer.</span><span class="sxs-lookup"><span data-stu-id="23772-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="23772-111">Hvis du vil ha mer informasjon, kan du se følgende emner:</span><span class="sxs-lookup"><span data-stu-id="23772-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="23772-112">Søke etter og slette meldinger</span><span class="sxs-lookup"><span data-stu-id="23772-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="23772-113">Søkepostboks</span><span class="sxs-lookup"><span data-stu-id="23772-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="23772-114">For postbokser som er på vent, må administratorer fjerne sperren før de kan slette elementer fra mappen Gjenopprettelige elementer.</span><span class="sxs-lookup"><span data-stu-id="23772-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="23772-115">Hvis du vil ha mer informasjon, kan du se [Slette elementer i mappen Gjenopprettelige elementer i skybaserte postbokser på vent](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="23772-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="23772-116">Hvis du vil hindre at mappen Gjenopprettelige elementer blir fullstendige, kan administratorer øke lagringsgrensen for mappen Gjenopprettelige elementer for postbokser som er på vent og konfigurere en postboksoppbevaringspolicy som flytter elementer fra mappen Gjenopprettelige elementer til brukerens arkivpostboks.</span><span class="sxs-lookup"><span data-stu-id="23772-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="23772-117">Se [Øke kvoten gjenopprettelige elementer for postbokser på vent](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="23772-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
