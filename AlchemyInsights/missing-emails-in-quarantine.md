---
title: Manglende e-post i karantene
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569554"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="ecc00-102">Manglende e-post i karantene"</span><span class="sxs-lookup"><span data-stu-id="ecc00-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="ecc00-103">Administratorer kan [vise, frigi eller slette disse meldingene.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="ecc00-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="ecc00-104">Hvis du vil åpne & for &, går du til [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="ecc00-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="ecc00-105">Hvis du vil åpne Karantene-siden direkte, går du til [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="ecc00-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="ecc00-106">Du kan søke etter følgende verdier:</span><span class="sxs-lookup"><span data-stu-id="ecc00-106">You can search by the following values:</span></span>  

- <span data-ttu-id="ecc00-107">**Meldings-ID**: Den globalt unike identifikatoren for meldingen.</span><span class="sxs-lookup"><span data-stu-id="ecc00-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="ecc00-108">Hvis du velger en melding i listen, vises **Details** **meldings-ID-verdien** i detalj-undermenyen som vises.</span><span class="sxs-lookup"><span data-stu-id="ecc00-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="ecc00-109">Administratorer kan bruke [meldingssporing](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) til å finne meldinger og de tilsvarende meldings-ID-verdiene.</span><span class="sxs-lookup"><span data-stu-id="ecc00-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="ecc00-110">**Avsenderens e-postadresse**: En enkelt avsenders e-postadresse.</span><span class="sxs-lookup"><span data-stu-id="ecc00-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="ecc00-111">**Mottaker-e-postadresse:** En enkelt mottakers e-postadresse.</span><span class="sxs-lookup"><span data-stu-id="ecc00-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="ecc00-112">**Emne**: Bruk hele emnet i meldingen.</span><span class="sxs-lookup"><span data-stu-id="ecc00-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="ecc00-113">Søket skiller ikke mellom store og små bokstaver.</span><span class="sxs-lookup"><span data-stu-id="ecc00-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="ecc00-114">Når du har angitt søkekriteriene, klikker du ![ Oppdater-knappen Oppdater for ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** å filtrere resultatene.  </span><span class="sxs-lookup"><span data-stu-id="ecc00-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="ecc00-115">Cmdletene du bruker til å vise og administrere meldinger og filer i karantene, er:</span><span class="sxs-lookup"><span data-stu-id="ecc00-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="ecc00-116">Slett karanteneMessage</span><span class="sxs-lookup"><span data-stu-id="ecc00-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="ecc00-117">Eksport-karanteneMessage</span><span class="sxs-lookup"><span data-stu-id="ecc00-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="ecc00-118">Få karanteneMessage</span><span class="sxs-lookup"><span data-stu-id="ecc00-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="ecc00-119">[Forhåndsvisning-KaranteneMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Vær oppmerksom på at denne cmdleten er bare for meldinger, ikke malware-filer fra ATP for SharePoint Online, OneDrive for Bedrifter eller Teams.</span><span class="sxs-lookup"><span data-stu-id="ecc00-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="ecc00-120">Slipp karanteneMessage</span><span class="sxs-lookup"><span data-stu-id="ecc00-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)