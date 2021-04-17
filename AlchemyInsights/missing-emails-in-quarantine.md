---
title: Manglende e-postmeldinger i karantene
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831743"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="ae904-102">Manglende e-postmeldinger i karantene"</span><span class="sxs-lookup"><span data-stu-id="ae904-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="ae904-103">Administratorer kan [vise, frigi eller slette disse meldingene.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="ae904-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="ae904-104">Hvis du vil åpne sikkerhetssenteret & samsvarssenteret, går du til [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="ae904-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="ae904-105">Hvis du vil åpne Karantenesiden direkte, går du til [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="ae904-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="ae904-106">Du kan søke etter følgende verdier:</span><span class="sxs-lookup"><span data-stu-id="ae904-106">You can search by the following values:</span></span>  

- <span data-ttu-id="ae904-107">**Meldings-ID:** Den globalt unike identifikatoren for meldingen.</span><span class="sxs-lookup"><span data-stu-id="ae904-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="ae904-108">Hvis du velger en melding i listen, vises  **Meldings-ID-verdien**  i  **detaljer-undermenyen**  som vises.</span><span class="sxs-lookup"><span data-stu-id="ae904-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="ae904-109">Administratorer kan bruke [meldingssporing til](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) å finne meldinger og tilhørende meldings-ID-verdier.</span><span class="sxs-lookup"><span data-stu-id="ae904-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="ae904-110">**Avsenderens e-postadresse:** En enkelt avsenders e-postadresse.</span><span class="sxs-lookup"><span data-stu-id="ae904-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="ae904-111">**E-postadresse for** mottaker: Én enkelt mottakers e-postadresse.</span><span class="sxs-lookup"><span data-stu-id="ae904-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="ae904-112">**Emne:** Bruk hele emnet i meldingen.</span><span class="sxs-lookup"><span data-stu-id="ae904-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="ae904-113">Søket skiller ikke mellom store og små bokstaver.</span><span class="sxs-lookup"><span data-stu-id="ae904-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="ae904-114">Når du har angitt søkekriteriene, klikker du ![ Oppdater-knappen ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Oppdater for** å filtrere resultatene.  </span><span class="sxs-lookup"><span data-stu-id="ae904-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="ae904-115">Cmdletene du bruker til å vise og behandle meldinger og filer i karantene, er:</span><span class="sxs-lookup"><span data-stu-id="ae904-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="ae904-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="ae904-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="ae904-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="ae904-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="ae904-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="ae904-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="ae904-119">[Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Vær oppmerksom på at denne cmdleten bare er for meldinger, ikke skadelig programvarefiler fra ATP for SharePoint Online, OneDrive for Business eller Teams.</span><span class="sxs-lookup"><span data-stu-id="ae904-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="ae904-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="ae904-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)