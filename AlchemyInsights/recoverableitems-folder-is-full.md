---
title: 1336 RecoverableItems mappen er full
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: cfcc69c1b3a59c73037d9a493af4ece86b7b7208
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762089"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="cb856-102">Gjenopprettbare elementer-mappen er full</span><span class="sxs-lookup"><span data-stu-id="cb856-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="cb856-103">For Exchange Online-postbokser i Office 365 er standard lagringsgrensen for mappen gjenopprettelige elementer 30 GB.</span><span class="sxs-lookup"><span data-stu-id="cb856-103">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="cb856-104">Lagringsgrensen for mappen gjenopprettelige elementer økes automatisk til 100 GB Hvis postboksen er plassert på rettstvist holder, eDiscovery sperring eller er knyttet til en oppbevaringspolicy for Office 365.</span><span class="sxs-lookup"><span data-stu-id="cb856-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>

<span data-ttu-id="cb856-105">Når mappen gjenopprettelige elementer når lagringsgrensen, påvirkes postboks-funksjonalitet på følgende måter:</span><span class="sxs-lookup"><span data-stu-id="cb856-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="cb856-106">Brukeren kan ikke slette elementer fra postboksen.</span><span class="sxs-lookup"><span data-stu-id="cb856-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="cb856-107">Administrerte Mappeassistent kan ikke slette elementer som er basert på kode for oppbevaring eller innstillinger for administrerte mapper.</span><span class="sxs-lookup"><span data-stu-id="cb856-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="cb856-108">Kopier på skrive siden beskyttelse prosessen kan ikke opprettholde versjoner av elementene som redigeres av brukeren for postbokser som har enkel gjenoppretting for elementer som er aktivert eller er satt på vent.</span><span class="sxs-lookup"><span data-stu-id="cb856-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="cb856-109">For postbokser som har postboksen overvåkes logging er aktivert, kan ingen postboks loggoppføringer for sporing av endringer ikke lagres i overvåking-undermappe i mappen gjenopprettbare elementer.</span><span class="sxs-lookup"><span data-stu-id="cb856-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="cb856-110">Administratorer kan bruke for postbokser som ikke er på vent og, den `Search-Mailbox -SearchDumpsterOnly -DeleteContent` i Exchange Online PowerShell til å slette elementer i mappen gjenopprettbare elementer.</span><span class="sxs-lookup"><span data-stu-id="cb856-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="cb856-111">Hvis du vil ha mer informasjon, kan du se følgende emner:</span><span class="sxs-lookup"><span data-stu-id="cb856-111">For more information, see the following topics:</span></span> 

- [<span data-ttu-id="cb856-112">Søke etter og slette meldinger</span><span class="sxs-lookup"><span data-stu-id="cb856-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="cb856-113">Søk-postboks</span><span class="sxs-lookup"><span data-stu-id="cb856-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="cb856-114">Administratorer må fjerne sperringen før de kan Slettede elementer fra mappen gjenopprettelige elementer for postbokser som er på vent.</span><span class="sxs-lookup"><span data-stu-id="cb856-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="cb856-115">Hvis du vil ha mer informasjon, kan du se [slette elementer i gjenopprettbare elementer-mappen for \\\cloud-based postbokser på holder](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="cb856-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="cb856-116">Administratorer kan øke lagringskapasiteten av gjenopprettbare elementer mappen for postbokser på hold og sette opp en oppbevaringspolicy på postboksen som flytter elementer fra mappen gjenopprettelige elementer til brukerens Arkiv for å hindre at mappen gjenopprettelige elementer blir full, postboks.</span><span class="sxs-lookup"><span data-stu-id="cb856-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="cb856-117">Se [øke gjenopprettbare elementer kvote for postbokser på hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="cb856-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
